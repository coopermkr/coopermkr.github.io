---
layout: default
title: Cooper Kimball-Rhines
description: PhD Candidate in Environmental Biology
---

<div class="top-nav">
  <nav>
    <a href="/index" class="nav-link">About Me</a>
    <a href="/research" class="nav-link">Research</a>
  </nav>
</div>

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
.top-nav {
  text-align: right;
  margin-bottom: 2rem;
  padding: 1rem 0;
  border-bottom: 1px solid #e0e0e0;
}

.top-nav nav {
  display: inline-block;
}

.nav-link {
  margin-left: 1rem;
  text-decoration: none;
  font-weight: bold;
  color: #0366d6;
}

.nav-link:hover {
  text-decoration: underline;
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
    <img src="/nevp.jpg" alt="Project 1">
  </div>
  <div class="research-text">
    <h2>Pine Barren Restoration</h2>
    <p>
      Pine barren ecosystems are globally rare, among the most biodiverse areas in the temperate United States, and on the brink of disappearance. The pine barren legume Lupinus perennis (sundial lupine) serves as host plant to over a dozen rare insect species, including the federally endangered Karner Blue Butterfly and state threatened Frosted Elfin Butterfly. When restoring pine barren species, managers must first establish strong plant populations. Traditional wisdom states that “local is best” when sourcing seeds for a restoration, but this advice fails to consider the adverse effects of propagating inbred plants with bottlenecked diversity. We worked with state and nonprofit ecosystem managers to sequence seven Northeast sites, representing the majority of extant L. perennis populations that are under conservation protection or have seed bank accessions in the region. We used a ddRAD method to obtain a filtered set of 46,000 SNPs. Population area did not predict observed population heterozygosity (p = 0.36) or inbreeding (p = 0.42). A mantel test with Pearson’s correlation indicates population isolation by geographic distance (r = 0.754, p = 0.001). We modeled the genetic effects of translocating seeds from 30 year old seed bank accessions and from the geographically closest population for the Vermont population. We find that seed translocations greatly benefit genetic diversity and effective population size in this population, while inaction will lead to likely extirpation of this species in the state of Vermont. Our results illustrate the complexity in selecting a healthy restoration source population and suggest that the “local is best” adage does not match practical reality. Dividing populations by political boundaries, especially when those boundaries arbitrarily divide historically connected ecosystems, should not be taken as a one-size fits all solution for restoration.
    </p>
  </div>
</div>

<div class="research-section">
  <div class="research-image">
    <img src="/manhattans.png" alt="Project 2">
  </div>
  <div class="research-text">
    <h2>Methylation</h2>
    <p>
      Methylation of CG motifs in many organisms is heritable, epimutable, and contributes to gene expression modulation. In plants, the rate of methylation epimutation is one million times faster than genetic mutation, making it one potential mechanism for rapid responses to the environment. Here we present a cost-effective approach using long-read Nanopore sequencing to simultaneously assess genetic and methylomic divergence and diversity in natural populations and demonstrate its utility in four populations of the the salt marsh plant Salicornia depressa. We find that pairwise genetic kinship between individuals is correlated with methylation profile (ρ = 0.3, p = 0.01). The four populations have similar genetic and methylation diversity across genomic windows, but highly genetically variable windows are uncorrelated with windows with high methylation density variation. Population divergence tests indicate that no genome windows are divergent in both genotype and methylation, as expected statistically if the two divergence types are uncorrelated. Our results suggest that regions of important genetic and methylation variation across populations are physically decoupled. Therefore, studies of complex trait evolution must consider the combined contributions of distinct genetic and methylation polymorphisms. Nanopore sequencing offers a promising avenue to reduce costs of such studies by obtaining genetic and methylation data concurrently. This approach could be a powerful tool to study species that lack standing genetic diversity, including crops and many plants of conservation concern. To encourage adoption and fill the gap of analysis tools available for Nanopore methylation data, we provide custom R scripts used for all methylation analyses.
    </p>
  </div>
</div>

<div class="research-section">
  <div class="research-image">
    <img src="/sal.jpg" alt="Project 3">
  </div>
  <div class="research-text">
    <h2>Genome Assembly</h2>
    <p>
      Salicornia depressa (American pickleweed) is the most widespread member of its salt-loving genus in North America. Pickleweeds typically colonize high marsh areas that tides make highly saline. Most other salt marsh plants cannot withstand the same salt pressure, so these bare patches are free from competitive pressures. Understanding the genetic origin of American Pickleweed’s high salinity adaptations has potential application to salt-tolerant agriculture and salt marsh conservation but requires genome resources to study. Salicornia depressa is a tetraploid species, which presents unique challenges to traditional genome assembly pipelines. We present a high-quality, chromosome-scale reference genome of S. depressa and the pipeline we used to assemble it. Our reference is phased to each of the tetraploid’s ancestral subgenomes with a scaffold N50 of 69.3 Mb, BUSCO completeness of 96.4%, and k-mer completeness of 98.4%. The subassemblies are evenly split, with subassembly A containing 56.7% and subassembly B containing 59.1% of genomic k-mers.  Our gene annotation identifies 80,883 genes and our methylome annotation contains 2.5 million methylated cytosines. We find that gene and methylation density are negatively correlated across the genome. We also assembled and annotated a chloroplast assembly which includes all expected photosystem, tRNA, and rRNA genes. We provide a guide to our successful assembly pipeline involving >30 programs. Our reference and annotation join resources for three other Salicornia species, allowing global scale ecological-evolutionary studies.
    </p>
  </div>
</div>

<div class="research-section">
  <div class="research-image">
    <img src="/shannonDID.png" alt="Project 4">
  </div>
  <div class="research-text">
    <h2>Policy Analysis</h2>
    <p>
      Conservation policymakers use an array of regulatory and legal mechanisms to conserve natural resources on public lands, yet there is no consensus on which mechanisms are most effective at conserving biodiversity. To address this gap, we systematically reviewed papers analysing changes in biodiversity after implementation of state-level conservation policies other than their Endangered Species Act in the United States. Our review reveals a major mismatch between statutory reality and academic literature, with only 12 published assessments of 13 conservation policies and their impacts on biodiversity from over five decades. We present an aggregative meta-summary of the policy mechanisms that have been assessed, the states where they have been implemented, and their impacts. To encourage future research comparing conservation mechanisms, we recommend standardization guidelines, including that policy assessments report the size of area affected and stakeholders involved in implementation of the policy and assess biodiversity changes (e.g. Shannon’s diversity index or population density of focal species) where applicable. As demonstration we present a case study analysis of a 1997 North Carolina amended law governing the state’s forestry council. Using a difference-in-difference method with data from the US Forest Service Forest Inventory and Analysis Database, we find the amendment had a positive effect on Shannon diversity of trees in state forests.
    </p>
  </div>
</div>
