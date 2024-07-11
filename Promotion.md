---
layout: page
title: Promotion!
permalink: /promotion/
---



<!-- MailerLite Universal -->
<script>
    (function(w,d,e,u,f,l,n){w[f]=w[f]||function(){(w[f].q=w[f].q||[])
    .push(arguments);},l=d.createElement(e),l.async=1,l.src=u,
    n=d.getElementsByTagName(e)[0],n.parentNode.insertBefore(l,n);})
    (window,document,'script','https://assets.mailerlite.com/js/universal.js','ml');
    ml('account', '908065');
</script>
<!-- End MailerLite Universal -->

<h2>
<div style="text-align: center; margin-top: 20px;">
    <a class="ml-onclick-form" href="javascript:void(0)" onclick="ml('show', '9R3d3M', true)" style="background-color: #007BFF; color: white; padding: 15px 32px; text-align: center; text-decoration: none; display: inline-block; font-size: 16px; border-radius: 8px;">
        <strong>📗 Sign up and get the e-book for free! 📗</strong>
    </a>
</div>
</h2>

<ebook-component></ebook-component>

<script>
    class EbookComponent extends HTMLElement {
        constructor() {
            super();
            this.attachShadow({ mode: 'open' });

            // Create a template for the shadow DOM
            const template = document.createElement('template');
            template.innerHTML = `
                <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.1.3/css/bootstrap.min.css">
                <style>
                    .container {
                        max-width: 800px;
                        margin: 50px auto;
                        padding: 20px;
                        background-color: #fff;
                        box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
                    }
                    .header {
                        text-align: center;
                        margin-bottom: 30px;
                    }
                    .header h2 {
                        font-size: 2.5rem;
                        color: #28a745; /* Changed color to green */
                    }
                    .header p {
                        font-size: 1.2rem;
                        color: #333;
                    }
                    .image-slider {
                        text-align: center;
                        margin: 20px 0;
                    }
                    .image-slider img {
                        max-width: 100%;
                        height: auto;
                        border-radius: 10px;
                    }
                    .image-slider button {
                        margin: 10px;
                        padding: 10px 20px;
                        font-size: 1rem;
                        border: none;
                        border-radius: 5px;
                        background-color: #007bff;
                        color: white;
                        cursor: pointer;
                    }
                    .content {
                        text-align: justify;
                        margin-bottom: 30px;
                    }
                    .content ul {
                        list-style: none;
                        padding: 0;
                    }
                    .content ul li {
                        margin-bottom: 10px;
                    }
                    .content ul li:before {
                        content: '✔';
                        margin-right: 10px;
                        color: #28a745; /* Changed color to green */
                    }
                    .buy-now {
                        text-align: center;
                        margin-top: 20px;
                    }
                    .buy-now a {
                        background-color: #28a745; /* Changed color to green */
                        color: white;
                        padding: 15px 32px;
                        text-align: center;
                        text-decoration: none;
                        display: inline-block;
                        font-size: 16px;
                        border-radius: 8px;
                    }
                    .footer {
                        text-align: center;
                        margin-top: 20px;
                        font-size: 0.9rem;
                    }
                    .footer a {
                        color: #007bff;
                    }
                </style>
                <div class="container">
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
                        <p>Are you struggling to keep your data science projects organized?</p>
                        <p>Do you find yourself losing track of your progress amidst the chaos of unstructured files and folders?</p>
                        <br>
                        <p><strong>Worry no more!</strong></p>
                        <br>
                        <p>In "Smart Structuring," Tomasz Guściora shares his decade-long experience in the data science field, peppered with humor and personal anecdotes, to help you streamline your projects and increase productivity.</p>
                        <br>
                        <br>
                        <h2><strong>What's Inside?</strong></h2>
                        <ul>
                            <li>Practical advice on project management for Python codebase</li>
                            <li>Humorous analogies and metaphors to simplify complex concepts</li>
                            <li>Clear explanations of coding best practices</li>
                            <li>Step-by-step guides with real-life examples</li>
                            <li>Valuable insights from Tomasz's personal experiences</li>
                        </ul>
                    </div>
					<h2>
					<div style="text-align: center; margin-top: 20px;">
					<a class="ml-onclick-form" href="javascript:void(0)" onclick="ml('show', '9R3d3M', true)" style="background-color: #007BFF; color: white; padding: 15px 32px; text-align: center; text-decoration: none; display: inline-block; font-size: 16px; border-radius: 8px;">
					<strong>📗 Sign up and get the e-book for free! 📗</strong>
					</a>
					</div>
					</h2>

                    <div class="footer text-center mt-4">
                        <p>Have questions? <a href="mailto:tomasz@demystifAI.blog">Contact the author</a></p>
                    </div>
                </div>
            `;

            // Append the template content to the shadow DOM
            this.shadowRoot.appendChild(template.content.cloneNode(true));

            // JavaScript for image slider
            const images = [
                '../../../assets/images/E001_landing/cover_title_hip.png',
                '../../../assets/images/E001_landing/bio.png',
                '../../../assets/images/E001_landing/toc1.png',
                '../../../assets/images/E001_landing/toc2.png',
            ];
            let currentIndex = 0;

            const showImage = (index) => {
                const imgElement = this.shadowRoot.getElementById('dynamic-image');
                imgElement.src = images[index];
            }

            this.shadowRoot.querySelector('button[onclick="nextImage()"]').addEventListener('click', () => {
                currentIndex = (currentIndex + 1) % images.length;
                showImage(currentIndex);
            });

            this.shadowRoot.querySelector('button[onclick="previousImage()"]').addEventListener('click', () => {
                currentIndex = (currentIndex - 1 + images.length) % images.length;
                showImage(currentIndex);
            });
        }
    }

    // Define the new element
    customElements.define('ebook-component', EbookComponent);
</script>
