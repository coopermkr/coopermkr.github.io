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
.container {
  display: flex;
  flex-wrap: wrap;
  align-items: stretch;
}

.research-photos {
  flex: 1 1 40%;
  max-width: 40%;
  display: flex;
  flex-direction: column;
}

.research-photos img {
  flex: 1;
  min-height: 120px;
  width: 100%;
  object-fit: cover;
  border-radius: 8px;
  margin-bottom: 1rem;
}

.research-content {
  flex: 2 1 65%;
}

research-section {
  margin-bottom: 2rem;
}

research-section h2 {
  margin-top 0;
}

.main-content {
  flex: 3 1 600px;
}

</style>

<!-- Lightbox modal -->
<div id="lightbox-modal" style="display:none; position:fixed; top:0; left:0; width:100%; height:100%; 
  background:rgba(0,0,0,0.8); z-index:9999; justify-content:center; align-items:center;">
  <img id="lightbox-image" src="" alt="Enlarged Image" style="max-width:90%; max-height:90%; border-radius:8px;" />
</div>

<script>
  document.addEventListener("DOMContentLoaded", function () {
    const modal = document.getElementById("lightbox-modal");
    const modalImg = document.getElementById("lightbox-image");

    document.querySelectorAll(".research-photos img").forEach(img => {
      img.style.cursor = "pointer";
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

<div class="container">
  <div class="research-photos">
    <img src="/manhattans.png">
    <img src="sal.jpg">
    <img src="/shannonDID.png">
  </div>

  <div class="research-content">
    <div class="research-section">
    <h2>Project 1</h2>
    <p>
	My research focuses on applying genomic techniques to inform conservation policy and practice. I mainly work with ecosystem managers to identify and answer questions about population structure, genetic diversity, and inbreeding in plants that form the foundation of their restoration projects. I work with short reads, long reads, DNA, RNA, and methylation to give managers the best recommendations I can. 
    </p>
    <p>
	When not in the lab, I am easily distracted by butterflies and will often interrupt myself to point one out if I know the species.
    </p>
  </div>

  <div class="research-section">
    <h2>Project 2</h2>
    <p>
	My research focuses on applying genomic techniques to inform conservation policy and practice. I mainly work with ecosystem managers to identify and answer questions about population structure, genetic diversity, and inbreeding in plants that form the foundation of their restoration projects. I work with short reads, long reads, DNA, RNA, and methylation to give managers the best recommendations I can. 
    </p>
    <p>
	When not in the lab, I am easily distracted by butterflies and will often interrupt myself to point one out if I know the species.
    </p>
  </div>

  <div class="research-section">
    <h2>Project 3</h2>
    <p>
	My research focuses on applying genomic techniques to inform conservation policy and practice. I mainly work with ecosystem managers to identify and answer questions about population structure, genetic diversity, and inbreeding in plants that form the foundation of their restoration projects. I work with short reads, long reads, DNA, RNA, and methylation to give managers the best recommendations I can. 
    </p>
    <p>
	When not in the lab, I am easily distracted by butterflies and will often interrupt myself to point one out if I know the species.
    </p>
  </div>
</div>
