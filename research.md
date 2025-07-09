---
layout: default
title: Cooper Kimball-Rhines
description: PhD Candidate in Environmental Biology
---

<nav style="text-align: right; margin-top: 0;">
  <a href="/index" style="margin-right: 1rem;">About Me</a>
  <a href="/research">Research</a>
</nav>

<style>
.research-section {
  display: flex;
  flex-direction: row;
  align-items: flex-start;
  justify-content: space-between;
  gap: 2rem;
  margin-bottom: 3rem;
  flex-wrap: nowrap;
}

.research-image {
  flex: 0 0 40%;
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
  flex: 1;
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

/* Mobile responsiveness */
@media (max-width: 768px) {
  .research-section {
    flex-direction: column;
  }
  .research-image,
  .research-text {
    max-width: 100%;
    flex: 1 1 100%;
  }
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

<div class="research-section">
  <div class="research-image">
    <img src="/manhattans.png" alt="Project 1">
  </div>
  <div class="research-text">
    <h2>Methylation</h2>
    <p>
      Description of Project 1. This section details the goals, collaborators, and outcomes of your research.
    </p>
  </div>
</div>

<div class="research-section">
  <div class="research-image">
    <img src="/sal.jpg" alt="Project 2">
  </div>
  <div class="research-text">
    <h2>Genome Assembly</h2>
    <p>
      Description of Project 2. This might cover methods, field sites, experimental designs, or data analysis.
    </p>
  </div>
</div>

<div class="research-section">
  <div class="research-image">
    <img src="/shannonDID.png" alt="Project 3">
  </div>
  <div class="research-text">
    <h2>Policy Analysis</h2>
    <p>
      Description of Project 3. You could also include links to publications or figures here.
    </p>
  </div>
</div>
