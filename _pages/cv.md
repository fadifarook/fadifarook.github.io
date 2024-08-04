---
layout: default
title: CV
cv_pdf: example_pdf.pdf
description: Detailed CV available for download.
nav: true
nav_order: 3
---

<!-- Page-specific content -->
<div class="container mt-5" role="main">
  <h1>{{ page.title }}</h1>
  <p>{{ page.description }}</p>
  
  <!-- Dynamic PDF Link -->
  {% if page.cv_pdf %}
    <a
      href="/assets/pdf/{{ page.cv_pdf | relative_url }}"
      target="_blank"
      rel="noopener noreferrer"
      class="float-right"
    >
      <i class="fa-solid fa-file-pdf"></i> View PDF
    </a>
  {% endif %}
</div>

<!-- JavaScript to automatically open the PDF -->
<script>
    window.onload = function() {
        var pdfUrl = "/assets/pdf/{{ page.cv_pdf | relative_url }}";
        console.log('Attempting to open PDF at:', pdfUrl); // Debugging output
        window.open(pdfUrl, '_blank');
    };
</script>
