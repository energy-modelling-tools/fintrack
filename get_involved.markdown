---
theme: jekyll-theme-primer
layout: sub-page
title: FinTrack
permalink: /contact/
---

<section class="bg-gray-light py-5 fade-in-center">
  <div class="container-lg p-responsive">
    <div class="text-center mb-5">
      <h2 class="alt-h2 mb-4">Get Involved</h2>
    </div>

    <div class="involvement-section mb-5">
      <h3 class="section-title text-center mb-4">Join the FinTrack community</h3>
      {% include forum_cta.html %}
      <!-- CMS:section id=get_involved_join_the_fintrack_community -->
      <p class="text-center lead mb-4">Join other FinTrack users in a shared space for questions, case studies, and updates on climate-finance tracking.</p>
      <!-- /CMS:section -->

      <div class="benefits-container">
        <div class="benefit-card text-center">
          <h5>Ask questions</h5>
          <!-- CMS:section id=get_involved_ask_questions -->
          <p class="text-gray">Share data questions, access-criteria issues, and modelling challenges with other practitioners.</p>
          <!-- /CMS:section -->
        </div>
        <div class="benefit-card text-center">
          <h5>Share applications</h5>
          <!-- CMS:section id=get_involved_share_applications -->
          <p class="text-gray">Publish country examples, visualisations, and lessons from using FinTrack in planning processes.</p>
          <!-- /CMS:section -->
        </div>
        <div class="benefit-card text-center">
          <h5>Stay updated</h5>
          <!-- CMS:section id=get_involved_stay_updated -->
          <p class="text-gray">Hear about training, Energy Modelling Platform events, and new FinTrack materials as they are released.</p>
          <!-- /CMS:section -->
        </div>
      </div>
    </div>
  </div>
</section>

<style>
.involvement-section {
  background: white;
  padding: 2rem;
  border-radius: 12px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
}
.section-title {
  color: #0366d6;
  font-size: 1.5rem;
  font-weight: 600;
  margin-bottom: 1.5rem;
  padding-bottom: 0.5rem;
  border-bottom: 2px solid #e1e4e8;
}
.benefits-container {
  display: flex;
  justify-content: center;
  align-items: stretch;
  gap: 2rem;
  flex-wrap: wrap;
  margin: 2rem auto 0;
  max-width: 900px;
}
.benefit-card {
  background: #f8f9fa;
  padding: 2rem 1rem;
  border-radius: 8px;
  border: 1px solid #e1e4e8;
  flex: 1;
  min-width: 250px;
  max-width: 280px;
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
