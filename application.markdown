---
theme: jekyll-theme-primer
layout: sub-page
title: FinTrack
permalink: /applications/
---
<section class="bg-gray-light container-lg p-responsive py-4 py-md-6 my-lg-6 fade-in-center">
  <div class="text-center fade-in-center">
    <h2 class="alt-h2 mb-4">FinTrack Applications</h2>
  </div>

  <div class="applications-content text-left">
    <!-- CMS:section id=application_fintrack_applications -->
    <p class="lead mb-4">FinTrack can support climate-finance planning across government, development partners, and research teams. Typical uses include:</p>
    <!-- /CMS:section -->

    <div class="applications-grid">
      <div class="application-category">
        <h3 class="category-title">Governments and planners</h3>
        <!-- CMS:section id=application_governments_and_planners -->
        <p>Use FinTrack to see how climate funds have been allocated, where indicative resources remain, and which access criteria apply when preparing national investment plans.</p>
        <!-- /CMS:section -->
      </div>

      <div class="application-category">
        <h3 class="category-title">Development partners</h3>
        <!-- CMS:section id=application_development_partners -->
        <p>Compare concessionality, eligibility, and historic use of climate funds to help countries identify larger volumes of accessible finance for sustainable transitions.</p>
        <!-- /CMS:section -->
      </div>
    </div>
  </div>
</section>

<section class="container-lg p-responsive py-4 py-md-6 my-lg-6">
  <div class="recommended-reading">
    <h2 class="alt-h2 text-center mb-4">Recommended Reading</h2>
    <!-- CMS:section id=application_recommended_reading -->
    <p class="text-center mb-5">For a broader analysis of applications and related work on FinTrack, see the following publications:</p>
    <!-- /CMS:section -->

    <div class="publications-list">
      {% for publication in site.data.publications %}
      <div class="publication-item mb-4 p-4 border border-gray-200 rounded">
        <h4 class="publication-title mb-2">
          <a href="{{ publication.url }}" target="_blank" class="text-decoration-none">
            {{ publication.title }}
          </a>
        </h4>
        <p class="publication-authors text-muted mb-2">
          {{ publication.authors }} ({{ publication.year }})
        </p>
        <p class="publication-journal mb-2">
          <em>{{ publication.journal }}</em>
        </p>
        <p class="publication-abstract text-justify">
          {{ publication.abstract }}
        </p>
      </div>
      {% endfor %}
    </div>
  </div>
</section>

<style>
.applications-content {
  max-width: 1200px;
  margin: 0 auto;
}
.applications-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
  margin-top: 2rem;
}
.application-category {
  background: white;
  padding: 2rem;
  border-radius: 12px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
}
.category-title {
  color: #0366d6;
  font-size: 1.3rem;
  font-weight: 600;
  margin-bottom: 1rem;
  padding-bottom: 0.5rem;
  border-bottom: 2px solid #e1e4e8;
}
.recommended-reading {
  max-width: 1000px;
  margin: 0 auto;
}
.publication-item {
  background: white;
  padding: 2rem;
  border-radius: 12px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
  border-left: 4px solid #0366d6;
}
.fade-in-center {
  opacity: 0;
  transform: translateY(30px);
  animation: fadeInUp 1.2s ease-out forwards;
}
@keyframes fadeInUp {
  to { opacity: 1; transform: translateY(0); }
}
</style>
