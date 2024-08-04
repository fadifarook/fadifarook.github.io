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
    <a href="fadifarook.github.io/assets/pdf/example_pdf.pdf" target="_blank">Click here to view the PDF</a>.
  </p>
</div>

<!-- JavaScript to automatically open the PDF -->
<script>
    window.onload = function() {
        var pdfUrl = "fadifarook.github.io/assets/pdf/example_pdf.pdf";
        window.open(pdfUrl, '_blank');
    };
</script>
