---
layout: page
title: E-book
permalink: /ebook/
---
<script type="text/javascript" src="https://payhip.com/payhip.js"></script>

<h2 style="text-align: center;"><strong>Smart Structuring</strong></h2>
<div style="display: flex; justify-content: center; align-items: center;">
    <p style="text-align: center;"><strong>A Guide to Efficiently Managing Data Science Projects in Python</strong></p>
</div>
<div style="display: flex; justify-content: center; align-items: center;">
    <br>
    <img id="dynamic-image" src="../../../assets/images/E001_landing/cover_title_hip.png" alt="Author photo" width="50%" height="auto">
</div>
<div style="text-align: center;">
    <button onclick="previousImage()">Previous</button>
    <button onclick="nextImage()">Next</button>
</div>
<br>
<p style="text-align: justify;">
    <strong>
        <ul>
            <li>Are you struggling to keep your data science projects organized?</li>
            <li>Do you find yourself losing track of your progress amidst the chaos of unstructured files and folders?</li>
        </ul>
        Worry no more! In "Smart Structuring," Tomasz Guściora shares his decade-long experience in the data science field, peppered with humor and personal anecdotes, to help you streamline your projects and increase productivity.
    </strong>
</p>
<br>
<div>
    <h2><strong>What's Inside?</strong></h2>
    <ul>
        <li>Practical advice on project management</li>
        <li>Humorous analogies and metaphors to simplify complex concepts</li>
        <li>Clear explanations of coding best practices</li>
        <li>Step-by-step guides with real-life examples</li>
        <li>Valuable insights from Tomasz's personal experiences</li>
    </ul>
</div>
<div style="text-align: center; margin-top: 20px;">
    <a href="https://payhip.com/b/4pz9P" target="_blank" style="background-color: #007BFF; color: white; padding: 15px 32px; text-align: center; text-decoration: none; display: inline-block; font-size: 16px; border-radius: 8px;">
        <strong>Buy Now</strong>
    </a>
</div>
<br>
<div style="text-align: center;">
    <p>Have questions? <a href="mailto:tomasz@demystifAI.blog">Contact the author</a></p>
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
</script>