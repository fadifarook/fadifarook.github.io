---
layout: default
title: CV
cv_pdf: example_pdf.pdf
description: Detailed CV available for download.
---

<!-- Page-specific content -->
<div class="container mt-5" role="main">
  <h1>{{ page.title }}</h1>
  <p>
    <a href="{{ page.cv_pdf | prepend: 'assets/pdf/' | relative_url}}" target="_blank">Click here to view the PDF</a>.
  </p>
</div>

<!-- JavaScript to automatically open the PDF -->
<script>
    window.onload = function() {
        var pdfUrl = "{{ page.cv_pdf | prepend: 'assets/pdf/' | relative_url}}";
        window.open(pdfUrl, '_blank');
    };
</script>
