<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8" />
        <meta http-equiv="X-UA-Compatible" content="IE=edge" />
        <title>ERSTE SCHRITTE MIT BRACKETS</title>
        <meta
            name="description"
            content="Ein interaktiver Wegweiser für die ersten Schritte mit Brackets."
        />
        <link rel="stylesheet" href="main.css" />
        <link rel="stylesheet" href="uikit-custom.css" />
        <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/gsap.min.js"></script>
        <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/ScrollTrigger.min.js"></script>
        <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/ScrollSmoother.min.js"></script>
        <script src="https://cdnjs.cloudflare.com/ajax/libs/animejs/3.2.2/anime.js"></script>
    </head>

  <body>
        <nav
            class="uk-navbar-container uk-navbar-transparent uk-padding-small"
            uk-navbar
        >
            <div class="uk-navbar-left">
                <a href="#" class="uk-logo">Mein Portfolio</a>
            </div>
            <div class="uk-navbar-right">
                <ul class="uk-navbar-nav">
                    <li><a href="#about">Über mich</a></li>
                    <li><a href="#projects">Projekte</a></li>
                    <li><a href="#contact">Kontakt</a></li>
                </ul>
            </div>
        </nav>
        <section
            class="uk-section uk-section-primary uk-flex uk-flex-center uk-flex-middle"
            style="height: 80vh"
        >
            <div class="uk-container uk-text-center"></div>
                <h1 class="uk-heading-medium my-text">Hallo, ich bin Max Mustermann</h1>
                <script>
                    anime
                        .timeline({ loop: true })
                        .add({
                            targets: ".my-text",
                            translateY: [100, 0],
                            easing: "easeOutExpo",
                            duration: 1400,
                        })
                        .add({
                            targets: ".my-text",
                            opacity: 0,
                            duration: 1000,
                            easing: "easeOutExpo",
                            delay: 1000,
                        });
                </script>
                <p class="uk-text-large">Mediengestalter & UI/UX Designer</p>
                <a href="#projects" class="uk-button uk-button-primary">Meine Arbeiten</a>
                <button id="animateBtn" class="uk-button uk-button-primary">Animate</button>
            </div>
        </section>

<section id="projects" class="uk-section uk-section-secondary">
            <div class="uk-container uk-padding-small">
                <h2 class="uk-heading-small"><span>Meine Projekte</span></h2>
                <div class="uk-grid-small uk-text-center uk-margin-large-top" uk-grid>
                    <div class="uk-width-2-3@m project-item">
                        <div class="uk-card uk-card-primary uk-card-hover uk-card-body">
                            <h3 class="uk-card-title">Projekt 1</h3>
                            <p>Beschreibung des Projekts.</p>
                        </div>
                    </div>
                    <div class="uk-width-1-3@m project-item">
                        <div class="uk-card uk-card-primary uk-card-hover uk-card-body"></div>
                            <h3 class="uk-card-title">Projekt 2</h3>
                            <p>Beschreibung des Projekts.</p>
                        </div>
                    </div>
                    <div class="uk-width-1-3@m project-item">
                        <div class="uk-card uk-card-primary uk-card-hover uk-card-body"></div>
                            <h3 class="uk-card-title">Projekt 3</h3>
                            <p>Beschreibung des Projekts.</p>
                        </div>
                    </div>
                    <div class="uk-width-2-3@m project-item"></div>
                        <div class="uk-card uk-card-primary uk-card-hover uk-card-body">
                            <h3 class="uk-card-title">Projekt 4</h3>
                            <p>Beschreibung des Projekts.</p>
                        </div>
                    </div>
                    <div class="uk-width-1-1 project-item"></div>
                        <div class="uk-card uk-card-primary uk-card-hover uk-card-body">
                            <h3 class="uk-card-title">Projekt 5</h3>
                            <p>Beschreibung des Projekts.</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

<script>
            document.querySelectorAll(".project-item").forEach((item) => {
                item.addEventListener("mouseenter", () => {
                    gsap.to(item, {
                        scale: 1.03,
                        duration: 0.3,
                        ease: "power1.out",
                    });
                });

                item.addEventListener("mouseleave", () => {
                    gsap.to(item, {
                        scale: 1,
                        duration: 0.3,
                        ease: "power1.in",
                    });
                });
            });
        </script>

<section id="contact" class="uk-section uk-section-secondary">
            <div class="uk-container uk-text-center">
                <h2>Kontakt</h2>
                <p>Schreib mir eine Nachricht!</p>
                <a href="mailto:max@email.com" class="uk-button uk-button-primary">E-Mail senden</a>
            </div>
        </section>

 <div class="timeline-container">
            <h2 class="uk-heading-small">Meine Berufliche Bahn</h2>
            <div class="timeline-item">
                <div class="uk-grid-small" uk-grid>
                    <div class="uk-width-1-4">
                        <div class="uk-card uk-card-default uk-card-body">
                            <h3>2020</h3>
                        </div>
                    </div>
                    <div class="uk-width-3-4">
                        <h3>Start in der IT Branche</h3>
                        <p>Ich habe meine Karriere als Junior Webentwickler begonnen.</p>
                    </div>
                </div>
            </div>
            <div class="timeline-item">
                <div class="uk-grid-small" uk-grid>
                    <div class="uk-width-1-4">
                        <div class="uk-card uk-card-default uk-card-body">
                            <h3>2022</h3>
                        </div>
                    </div>
                    <div class="uk-width-3-4">
                        <h3>Teamleiter</h3>
                        <p>Ich wurde zum Teamleiter in meinem Unternehmen befördert und leitete ein kleines Entwicklungsteam.</p>
                    </div>
                </div>
            </div>
            <div class="timeline-item">
                <div class="uk-grid-small" uk-grid>
                    <div class="uk-width-1-4">
                        <div class="uk-card uk-card-default uk-card-body">
                            <h3 id="timeline-item-2024">2024</h3>
                        </div>
                    </div>
                    <div class="uk-width-3-4">
                        <h3>Senior Entwickler</h3>
                        <p>Ich wurde zum Senior Webentwickler befördert und arbeite nun an großen Projekten.</p>
                    </div>
                </div>
            </div>
        </div>

  <style>
            @import url("https://cdn.jsdelivr.net/npm/uikit@3.9.1/dist/css/uikit.min.css");
            @import url("https://fonts.googleapis.com/css2?family=Syne:wght@700&display=swap");
            @import url("https://fonts.googleapis.com/css2?family=Helvetica&display=swap");

            :root {
                --primary-color: #000000;
                --secondary-color: #d0bcff;
                --background-color: #f5f5f5;
                --text-color: #000000;
                --card-background: #ffffff;
                --font-main: "Helvetica", sans-serif;
                --font-heading: "Syne", sans-serif;
            }

            h1,
            h2,
            h3,
            h4,
            h5,
            h6,
            .uk-heading-small,
            .uk-heading-medium,
            .uk-heading-large {
                font-family: var(--font-heading);
                color: red !important;
            }

            html {
                background: #ff0000;
                background-image: linear-gradient(
                    270deg,
                    rgb(0, 252, 252) 0%,
                    rgb(52, 255, 255) 100%
                );
                -webkit-font-smoothing: antialiased;
                font-family: var(--font-main);
            }

            .uk-navbar-container {
                background-color: var(--primary-color);
            }

            body {
                background-color: var(--background-color);
                color: var(--text-color);
                font-family: var(--font-main);
            }

            .uk-card,
            .uk-button {
                border-radius: 3vw;
                transition: 1200ms ease;
            }

            .uk-card:hover {
                border-radius: 6vw;
            }

            .uk-card-primary {
                background-color: var(--primary-color);
            }

            .uk-section.uk-section-primary {
                background-color: var(--primary-color);
                color: red;
            }

            .uk-section-secondary {
                background-color: rgb(235, 235, 235) !important;
                color: blue !important;
            }

            body .uk-section.uk-section-secondary {
                background-color: rgb(235, 235, 235) !important;
                color: blue !important;
            }

            .smooth-wrapper {
                overflow: hidden;
            }

            .smooth-content {
                padding: 100px;
            }

            .timeline-container {
                max-width: 800px;
                margin: 0 auto;
            }

            .timeline-item {
                background-color: #fff;
                border: 1px solid #ddd;
                padding: 20px;
                margin-bottom: 20px;
                border-radius: 8px;
                opacity: 0;
                transform: translateY(100px);
            }

            .timeline-item h3 {
                font-size: 24px;
                color: #333;
            }

            .timeline-item p {
                color: #777;
            }

            .timeline-item .uk-grid {
                display: flex;
                justify-content: space-between;
            }

            .timeline-item .uk-card-body {
                background: #f4f4f4;
                border-radius: 5px;
            }
        </style>

 <script>
            gsap.registerPlugin(ScrollTrigger);

            const timeline = gsap.timeline({
                scrollTrigger: {
                    trigger: ".timeline-container",
                    start: "top 80%",
                    end: "bottom 20%",
                    scrub: true,
                    markers: false,
                },
            });

            timeline.to(".timeline-item", {
                opacity: 1,
                y: 0,
                stagger: 0.3,
                duration: 1,
                ease: "power2.out",
            });
        </script>

<script src="https://cdn.jsdelivr.net/npm/uikit@3.22.4/dist/js/uikit.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/uikit@3.22.4/dist/js/uikit-icons.min.js"></script>
</body>
</html>
