---
layout: page
title: Portfolio
permalink: /portfolio/
---

# Technical Writing Portfolio

Below are samples of my technical writing work. Click on the tabs to view different examples.

<div class="tabs">
  <div class="tab-buttons">
    <button class="tab-button active" onclick="openTab(event, 'api-docs')">API Documentation</button>
    <button class="tab-button" onclick="openTab(event, 'user-guides')">User Guides</button>
    <button class="tab-button" onclick="openTab(event, 'explanatory')">Explanatory Content</button>
    <button class="tab-button" onclick="openTab(event, 'tutorials')">Tutorials</button>
    <button class="tab-button" onclick="openTab(event, 'technical-blogs')">Technical Blogs</button>
  </div>

  <div id="api-docs" class="tab-content active">
    <h2>API Documentation Examples</h2>
    <p>These samples demonstrate my ability to document complex APIs in a clear, developer-friendly manner.</p>
    
    <div class="portfolio-item">
      <h3>Viam Data Client API Reference</h3>
      <p>Comprehensive documentation for the Viam Data Client API, including authentication methods, request formats, and response examples.</p>
      <div class="pdf-container">
        <iframe src="/assets/pdfs/data_client.pdf" width="100%" height="500px"></iframe>
      </div>
    </div>
    <div class="portfolio-item">
      <h3>Viam Vision Service API Reference</h3>
      <p>Comprehensive documentation for the Viam Computer Vision Service API, including authentication methods, request formats, and response examples.</p>
      <div class="pdf-container">
        <iframe src="/assets/pdfs/vision_service.pdf" width="100%" height="500px"></iframe>
      </div>
    </div>
  </div>

  <div id="user-guides" class="tab-content">
    <h2>User Guide Examples</h2>
    <p>These guides showcase my ability to create clear instructional content for end-users.</p>
    
    <div class="portfolio-item">
      <h3>Create a Dataset</h3>
      <p>Step-by-step instructions for creating a dataset using the Viam platform.</p>
      <div class="pdf-container">
        <iframe src="/assets/pdfs/create_dataset.pdf" width="100%" height="500px"></iframe>
      </div>
    </div>

    <div class="portfolio-item">
      <h3>Filter before Sync</h3>
      <p>Step-by-step instructions for filtering data before syncing it to the Viam cloud.</p>
      <div class="pdf-container">
        <iframe src="/assets/pdfs/filter_before_sync.pdf" width="100%" height="500px"></iframe>
      </div>
    </div>
  </div>

  <div id="explanatory" class="tab-content">
    <h2>Explanatory Content Example</h2>
    <p>This guide showcases my ability to break down complex technical concepts.</p>
    
    <div class="portfolio-item">
      <h3>How Sync Works</h3>
      <p>How data is synced to the cloud in the Viam platform.</p>
      <div class="pdf-container">
        <iframe src="/assets/pdfs/how_sync_works.pdf" width="100%" height="500px"></iframe>
      </div>
    </div>
  </div>

  <div id="tutorials" class="tab-content">
    <h2>Tutorial Examples</h2>
    <p>These tutorials demonstrate my ability to guide users through complex technical processes.</p>
    
    <div class="portfolio-item">
      <h3>Navigate with a Rover Base</h3>
      <p>A tutorial for experienced developers working with the Viam platform to navigate with a rover base.</p>
      <div class="pdf-container">
        <iframe src="/assets/pdfs/navigate.pdf" width="100%" height="500px"></iframe>
      </div>
    </div>

    <div class="portfolio-item">
      <h3>Make a Plant Watering Robot</h3>
      <p>A beginner-friendly tutorial for new developers working with the Viam platform.</p>
      <div class="pdf-container">
        <iframe src="/assets/pdfs/plant_watering.pdf" width="100%" height="500px"></iframe>
      </div>
    </div>
  </div>

  <div id="technical-blogs" class="tab-content">
  <h2>Technical Blog Examples</h2>
  <p>These blog posts showcase my ability to explain technical concepts in an engaging way.</p>
  
  <div class="portfolio-item">
    <h3>A Day in My Life as a Technical Writer</h3>
    <p>An exploration of a day in my life as a technical writer.</p>
    <a href="https://nalmadi.github.io/student-interview-Sierra-Guequierre/" target="_blank" class="blog-link">
      <div class="blog-card">
        <div class="blog-image">
          <img src="/assets/images/blog_thumbnail_1.jpg" alt="Blog thumbnail">
        </div>
        <div class="blog-info">
          <p class="blog-date">Published: June 20, 2024</p>
          <p class="blog-excerpt">This post is part of a spotlight series highlighting the work of exceptional students and alumni. The series aims to facilitate knowledge sharing on topics such as internships, jobs, entrepreneurship, and graduate school...</p>
          <span class="read-more">Read Full Article →</span>
        </div>
      </div>
    </a>
  </div>
  
  <div class="portfolio-item">
    <h3>Plant Watering Robot with a Raspberry Pi</h3>
    <p>How to build a plant watering robot with a Raspberry Pi.</p>
    <a href="https://www.hackster.io/sierraguequierre/plant-watering-robot-with-a-raspberry-pi-acbea2" target="_blank" class="blog-link">
      <div class="blog-card">
        <div class="blog-image">
          <img src="/assets/images/blog_thumbnail_2.png" alt="Blog thumbnail">
        </div>
        <div class="blog-info">
          <p class="blog-date">Published: October 3rd, 2023</p>
          <p class="blog-excerpt">With a Raspberry Pi and some cheap, basic hardware, you can keep your plants healthy and happy from anywhere in the world...</p>
          <span class="read-more">Read Full Article →</span>
        </div>
      </div>
    </a>
  </div>
  </div>
</div>

<!-- Add tab functionality -->
<script>
function openTab(evt, tabName) {
  var i, tabContent, tabButtons;
  
  // Hide all tab content
  tabContent = document.getElementsByClassName("tab-content");
  for (i = 0; i < tabContent.length; i++) {
    tabContent[i].className = tabContent[i].className.replace(" active", "");
  }
  
  // Remove "active" class from all tab buttons
  tabButtons = document.getElementsByClassName("tab-button");
  for (i = 0; i < tabButtons.length; i++) {
    tabButtons[i].className = tabButtons[i].className.replace(" active", "");
  }
  
  // Show the current tab and add "active" class to the button
  document.getElementById(tabName).className += " active";
  evt.currentTarget.className += " active";
}
</script>

<!-- Add custom CSS for tabs and PDF containers -->
<style>
.tabs {
  width: 100%;
  margin: 2rem 0;
}

.tab-buttons {
  display: flex;
  flex-wrap: wrap;
  margin-bottom: 1rem;
}

.tab-button {
  background-color: #f1f1f1;
  border: none;
  outline: none;
  cursor: pointer;
  padding: 0.8rem 1.2rem;
  margin-right: 0.5rem;
  margin-bottom: 0.5rem;
  border-radius: 4px;
  font-weight: 500;
  transition: background-color 0.3s;
}

.tab-button:hover {
  background-color: #ddd;
}

.tab-button.active {
  background-color: #0366d6;
  color: white;
}

.tab-content {
  display: none;
  padding: 1rem;
  border: 1px solid #ddd;
  border-radius: 4px;
}

.tab-content.active {
  display: block;
}

.portfolio-item {
  margin-bottom: 2rem;
}

.pdf-container {
  margin: 1rem 0;
  border: 1px solid #ddd;
  border-radius: 4px;
  overflow: hidden;
}
</style>