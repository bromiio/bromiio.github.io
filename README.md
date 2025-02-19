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
    <script src="anime.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/animejs/3.2.2/anime.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.9.1/ScrollTrigger.min.js"></script>
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
      <div class="uk-container uk-text-center">
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
              targets: ".my-text ",
              opacity: 0,
              duration: 1000,
              easing: "easeOutExpo",
              delay: 1000,
            });
        </script>
        <p class="uk-text-large">Mediengestalter & UI/UX Designer</p>
        <a href="#projects" class="uk-button uk-button-primary"
          >Meine Arbeiten</a
        >
        <button id="animateBtn" class="uk-button uk-button-primary">
          Animate
        </button>
      </div>
    </section>

  <section id="projects" class="uk-section uk-section-secondary">
      <div class="uk-container uk-padding-small">
        <h2 class="uk-heading-small"><span>Meine Projekte</span></h2>
        <div class="uk-grid-small uk-text-center uk-margin-large-top" uk-grid>
          <!-- First grid item: bigger size -->
          <div class="uk-width-2-3@m project-item">
            <div class="uk-card uk-card-primary uk-card-hover uk-card-body">
              <h3 class="uk-card-title">Projekt 1</h3>
              <p>Beschreibung des Projekts.</p>
            </div>
          </div
          <div class="uk-width-1-3@m project-item">
            <div class="uk-card uk-card-primary uk-card-hover uk-card-body">
              <h3 class="uk-card-title">Projekt 2</h3>
              <p>Beschreibung des Projekts.</p>
            </div>
          </div> <!-- First grid item: bigger size -->
          <div class="uk-width-1-3@m project-item">
            <div class="uk-card uk-card-primary uk-card-hover uk-card-body">
              <h3 class="uk-card-title">Projekt 1</h3>
              <p>Beschreibung des Projekts.</p>
            </div>
          </div>
 <div class="uk-width-2-3@m project-item">
            <div class="uk-card uk-card-primary uk-card-hover uk-card-body">
              <h3 class="uk-card-title">Projekt 2</h3>
              <p>Beschreibung des Projekts.</p>
            </div>
          </div>
          <div class="uk-width-1-1 project-item">
            <div class="uk-card uk-card-primary uk-card-hover uk-card-body">
              <h3 class="uk-card-title">Projekt 3</h3>
              <p>Beschreibung des Projekts.</p>
            </div>
          </div>
        </div>
      </div>
    </section>

 <script>
      // GSAP hover effect for scaling the grid item
      document.querySelectorAll(".project-item").forEach((item) => {
        item.addEventListener("mouseenter", () => {
          // GSAP animation for the hover effect (scaling)
          gsap.to(item, {
            scale: 1.03, // Scale the item up to 110%
            duration: 0.3, // Duration of the animation
            ease: "power1.out", // Smooth easing for the animation
          });
        });

        item.addEventListener("mouseleave", () => {
          // GSAP animation to revert back to the original size
          gsap.to(item, {
            scale: 1, // Reset scale to 100%
            duration: 0.3, // Duration of the reset animation
            ease: "power1.in", // Smooth easing for the reset
          });
        });
      });
    </script>

 <section id="contact" class="uk-section uk-section-secondary">
      <div class="uk-container uk-text-center">
        <h2>Kontakt</h2>
        <p>Schreib mir eine Nachricht!</p>
        <a href="mailto:max@email.com" class="uk-button uk-button-primary"
          >E-Mail senden</a
        >
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
  <div class="timeline-item" role="region" aria-labelledby="timeline-item-2024"></div>
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

</body>
    
 <script>
        // Register ScrollTrigger with GSAP
        gsap.registerPlugin(ScrollTrigger);
    
        // GSAP Timeline Animation
        const timeline = gsap.timeline({
          scrollTrigger: {
            trigger: ".timeline-container", // When the container enters the viewport
            start: "top 80%", // Trigger animation when the container is 80% visible
            end: "bottom 20%", // End animation when the container is 20% from the bottom
            scrub: true, // Smoothly scrubs through the timeline
            markers: false, // Disable the markers
          }
        });
    
        // Animate timeline items sequentially
        timeline
          .to(".timeline-item", {
            opacity: 1,
            y: 0,  // Move items into position
            stagger: 0.3, // Add a small delay between items
            duration: 1,
            ease: "power2.out",
          });
      </script>
<!-- UIkit JS -->
 <script src="https://cdn.jsdelivr.net/npm/uikit@3.22.4/dist/js/uikit.min.js"></script>
 <script src="https://cdn.jsdelivr.net/npm/uikit@3.22.4/dist/js/uikit-icons.min.js"></script>


  </body>
</html>
