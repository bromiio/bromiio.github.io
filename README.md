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

<style>/* Timeline container */

/* Import UIkit CSS */
@import url("https://cdn.jsdelivr.net/npm/uikit@3.9.1/dist/css/uikit.min.css");
@import url("https://fonts.googleapis.com/css2?family=Syne:wght@700&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Helvetica&display=swap");

/* Global Styles for Layouts and Fonts */
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
  font-family: var(--font-heading); /* Apply Syne to headings */
  color: red !important;
}

/* Ensure the font is applied globally */
html {
  background: #ff0000;
  background-image: linear-gradient(
    270deg,
    rgb(0, 252, 252) 0%,
    rgb(52, 255, 255) 100%
  );
  -webkit-font-smoothing: antialiased;
  font-family: var(--font-main); /* Apply default font globally */
}

.uk-navbar-container {
  background-color: var(--primary-color);
}

/* Override UIkit’s default styles with custom values */
body {
  background-color: var(--background-color);
  color: var(--text-color);
  font-family: var(--font-main); /* Ensure body uses Helvetica as default */
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
  background-color: rgb(
    235,
    235,
    235
  ) !important; /* Ensure the background is applied */
  color: blue !important; /* Ensure text color is applied */
}

/* You can add specific styles for the .uk-section-secondary class to target it more precisely */
body .uk-section.uk-section-secondary {
  background-color: rgb(235, 235, 235) !important;
  color: blue !important;
}

.smooth-wrapper {
  overflow: hidden; /* This is important for the smooth scroll to work */
}
.smooth-content {
  padding: 100px; /* Add some padding to make it scrollable */
}




.timeline-container {
    max-width: 800px;
    margin: 0 auto;
  }

  /* Individual timeline block */
  .timeline-item {
    background-color: #fff;
    border: 1px solid #ddd;
    padding: 20px;
    margin-bottom: 20px;
    border-radius: 8px;
    opacity: 0; /* Make items invisible initially */
    transform: translateY(100px); /* Start off screen */
  }

  /* Timeline heading */
  .timeline-item h3 {
    font-size: 24px;
    color: #333;
  }

  .timeline-item p {
    color: #777;
  }

  /* Timeline item positioning */
  .timeline-item .uk-grid {
    display: flex;
    justify-content: space-between;
  }

  .timeline-item .uk-card-body {
    background: #f4f4f4;
    border-radius: 5px;
  }</style>
    
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
