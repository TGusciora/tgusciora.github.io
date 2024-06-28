---
layout: page
title: E-book
permalink: /ebook/
---
<script type="text/javascript" src="https://payhip.com/payhip.js"></script>

<div id="ebook-container">
    <div class="header text-center mb-4">
        <h2><strong>Smart Structuring</strong></h2>
        <p><strong>A Guide to Efficiently Managing Data Science Projects in Python</strong></p>
    </div>

    <div class="image-slider text-center mb-4">
        <img id="dynamic-image" src="../../../assets/images/E001_landing/cover_title_hip.png" alt="Book cover" class="img-fluid rounded" style="max-width: 100%; height: auto;">
        <div class="mt-3">
            <button class="btn btn-primary me-2" onclick="previousImage()">Previous</button>
            <button class="btn btn-primary" onclick="nextImage()">Next</button>
        </div>
    </div>

    <div class="content mb-4">
        <p><strong>Are you struggling to keep your data science projects organized? Do you find yourself losing track of your progress amidst the chaos of unstructured files and folders?</strong></p>
        <p><strong>Worry no more! In "Smart Structuring," Tomasz Guściora shares his decade-long experience in the data science field, peppered with humor and personal anecdotes, to help you streamline your projects and increase productivity.</strong></p>
        <h2><strong>What's Inside?</strong></h2>
        <ul>
            <li>Practical advice on project management</li>
            <li>Humorous analogies and metaphors to simplify complex concepts</li>
            <li>Clear explanations of coding best practices</li>
            <li>Step-by-step guides with real-life examples</li>
            <li>Valuable insights from Tomasz's personal experiences</li>
        </ul>
    </div>

    <div class="text-center my-4">
        <a href="https://payhip.com/b/4pz9P" target="_blank" class="btn btn-primary btn-lg"><strong>Buy Now</strong></a>
    </div>

    <div class="footer text-center mt-4">
        <p>Have questions? <a href="mailto:tomasz@demystifAI.blog">Contact the author</a></p>
    </div>
</div>

<script>
    const images = [
        '../../../assets/images/E001_landing/cover_title_hip.png',
        '../../../assets/images/E001_landing/bio.png',
        '../../../assets/images/E001_landing/toc1.png',
        '../../../assets/images/E001_landing/toc2.png',
    ];
    let currentIndex = 0;

    function showImage(index) {
        const imgElement = document.getElementById('dynamic-image');
        imgElement.src = images[index];
    }

    function nextImage() {
        currentIndex = (currentIndex + 1) % images.length;
        showImage(currentIndex);
    }

    function previousImage() {
        currentIndex = (currentIndex - 1 + images.length) % images.length;
        showImage(currentIndex);
    }

    // Load Bootstrap CSS and apply it to the ebook-container
    var link = document.createElement("link");
    link.rel = "stylesheet";
    link.href = "https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.1.3/css/bootstrap.min.css";
    document.getElementById("ebook-container").appendChild(link);
</script>
