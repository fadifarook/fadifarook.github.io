---
layout: page
title: cv
permalink: /assets/pdf//Fadi_CV.pdf
nav: true
nav_order: 3
cv_pdf: Fadi_CV.pdf
---

<a href="/assets/pdf/{{ page.cv_pdf | relative_url }}">Click here for the PDF</a>

<body>
    <!-- JavaScript to automatically open the PDF -->
    <script>
        window.onload = function() {
            var pdfUrl = "/assets/pdf/{{ page.cv_pdf | relative_url }}";
            console.log('Attempting to open PDF at:', pdfUrl); // Debugging output
            window.open(pdfUrl, '_blank');
        };
    </script>
</body>