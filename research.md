---
layout: default
title: Cooper Kimball-Rhines
description: PhD Candidate in Environmental Biology
---

<nav style="text-align: right; margin-top: 0;">
  <a href="/index" style="margin-right: 1rem;">About Me</a>
  <a href="/research">Research</a>
</nav>

<h1>Research</h1>

<style>
.research-section {
  display: flex;
  flex-wrap: wrap;
  margin-bottom: 2rem;
  gap: 1.5rem;
  align-items: flex-start;
}

.research-image {
  flex: 1 1 40%;
  max-width: 40%;
}

.research-image img {
  width: 100%;
  height: auto;
  object-fit: cover;
  border-radius: 8px;
  cursor: pointer;
}

.research-text {
  flex: 1 1 58%;
}

#lightbox-modal {
  display: none;
  position: fixed;
  top: 0; left: 0;
  width: 100%; height: 100%;
  background: rgba(0, 0, 0, 0.85);
  z-index: 9999;
  justify-content: center;
  align-items: center;
}

#lightbox-modal img {
  max-width: 90%;
  max-height: 90%;
  border-radius: 8px;
}
</style>

<!-- Lightbox Modal -->
<div id="lightbox-modal">
  <img id="lightbox-image" src="" alt="Expanded Image" />
</div>

<script>
  document.addEventListener("DOMContentLoaded", function () {
    const modal = document.getElementById("lightbox-modal");
    const modalImg = document.getElementById("lightbox-image");

    document.querySelectorAll(".research-image img").forEach(img => {
      img.addEventListener("click", () => {
        modal.style.display = "flex";
        modalImg.src = img.src;
        modalImg.alt = img.alt;
      });
    });

    modal.addEventListener("click", () => {
      modal.style.display = "none";
    });
  });
</script>

<!-- Project 1 -->
<div class="research-section">
  <div class="research-image">
    <img src="/manhattans.png">
  </div>
  <div class="research-text">
    <h2>Methylation</h2>
    <p>
      Description of Project 1. You can include collaborators, goals, methods, and key findings.
    </p>
  </div>
</div>

<!-- Project 2 -->
<div class="research-section">
  <div class="research-image">
    <img src="/sal.jpg">
  </div>
  <div class="research-text">
    <h2>Genome Assembly</h2>
    <p>
      Description of Project 2. Fieldwork, lab work, modeling, and interesting outcomes can go here.
    </p>
  </div>
</div>

<!-- Project 3 -->
<div class="research-section">
  <div class="research-image">
    <img src="shannonDID.png">
  </div>
  <div class="research-text">
    <h2>Policy Analysis</h2>
    <p>
      Description of Project 3. Highlight significance, contributions, or links to publications.
    </p>
  </div>
</div>
