# Bethany-Peirson.github.io
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>The Pilates Garden — Mat Pilates Outdoors</title>

  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Inria+Serif:wght@700&family=Intel+One+Mono:wght@300&family=Inria+Sans:wght@400&display=swap" rel="stylesheet">

  <style>
    :root {
      --cream: #F3EDE5;
      --green: #212C16;
      --accent: #563D1A;

      --heading-serif: 'Inria Serif', serif;
      --heading-mono: 'Intel One Mono', monospace;
      --body-font: 'Inria Sans', sans-serif;

      --button-radius: 170px;
      --button-padding: 8px 50px;
    }

    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      background: var(--cream);
      color: var(--green);
      font-family: var(--body-font);
      font-size: 14px;
      line-height: 20px;
    }

    main {
      max-width: 1200px;
      margin: 0 auto;
    }

    /* HEADER */
    .site-header {
      max-width: 1200px;
      margin: 0 auto;
      padding: 20px 40px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .logo {
      text-decoration: none;
      color: var(--green);
      font-family: var(--heading-serif);
      display: flex;
      flex-direction: column;
      line-height: 1.1;
      font-size: 22px;
    }

    .main-nav {
      display: flex;
      gap: 30px;
      align-items: center;
    }

    .main-nav a {
      text-decoration: none;
      color: var(--green);
      font-size: 16px;
    }

    .nav-button {
      background: var(--green);
      color: var(--cream);
      padding: var(--button-padding);
      border-radius: var(--button-radius);
      font-size: 16px;
    }

    /* HERO */
    .hero {
      display: grid;
      grid-template-columns: 1.1fr 0.9fr;
      gap: 40px;
      padding: 60px 40px;
      align-items: center;
    }

    .hero-content .eyebrow {
      font-family: var(--heading-mono);
      font-size: 18px;
      letter-spacing: 0.05em;
      text-transform: uppercase;
      margin-bottom: 10px;
    }

    .hero-content h1 {
      font-family: var(--heading-serif);
      font-size: 40px;
      margin: 0 0 10px;
    }

    .hero-subtitle {
      font-family: var(--heading-mono);
      font-size: 22px;
      margin-bottom: 15px;
    }

    .hero-description {
      max-width: 420px;
      margin-bottom: 25px;
    }

    .button {
      display: inline-block;
      text-decoration: none;
      background: var(--green);
      color: var(--cream);
      padding: var(--button-padding);
      border-radius: var(--button-radius);
      font-size: 18px;
    }

    .hero-image img {
      width: 100%;
      height: auto;
      border-radius: 12px;
      object-fit: cover;
    }

    /* SECTION HEADING */
    .section-heading {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 16px;
      margin: 40px 0 20px;
    }

    .section-heading span {
      flex: 1;
      height: 1px;
      background: var(--green);
      max-width: 120px;
    }

    .section-heading h2 {
      font-family: var(--heading-serif);
      font-size: 26px;
      margin: 0;
    }

    /* CLASSES */
    .classes-section {
      background: var(--green);
      color: var(--cream);
      padding: 40px 40px 60px;
    }

    .classes-section .section-heading span {
      background: var(--cream);
    }

    .classes-section .section-heading h2 {
      color: var(--cream);
    }

    .class-grid {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 24px;
    }

    .class-card {
      background: var(--green);
      border: 1px solid var(--cream);
      border-radius: 10px;
      padding: 20px;
    }

    .class-card img {
      width: 100%;
      height: 160px;
      object-fit: cover;
      border-radius: 8px;
      margin-bottom: 12px;
    }

    .class-card h3 {
      font-family: var(--heading-serif);
      font-size: 20px;
      margin: 0 0 8px;
    }

    .class-card p {
      font-size: 13px;
      margin-bottom: 10px;
    }

    .class-card a {
      color: var(--cream);
      font-size: 13px;
      text-decoration: underline;
    }

    /* ABOUT STYLE */
    .about-style {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 40px;
      padding: 60px 40px;
      align-items: center;
    }

    .about-style img {
      width: 100%;
      height: auto;
      border-radius: 12px;
      object-fit: cover;
    }

    .about-style h2 {
      font-family: var(--heading-serif);
      font-size: 28px;
      margin: 0 0 10px;
    }

    .about-style h3 {
      font-family: var(--heading-mono);
      font-size: 20px;
      font-weight: 300;
      margin: 0 0 18px;
    }

    .about-style p {
      max-width: 420px;
      margin-bottom: 24px;
    }

    .about-style .button {
      font-size: 16px;
    }

    /* LOCATION */
    .location-section {
      display: grid;
      grid-template-columns: 1.1fr 0.9fr;
      gap: 40px;
      padding: 60px 40px;
      align-items: center;
      background: var(--green);
      color: var(--cream);
    }

    .location-section h2 {
      font-family: var(--heading-serif);
      font-size: 26px;
      margin: 0 0 8px;
    }

    .location-section h3 {
      font-family: var(--heading-mono);
      font-size: 20px;
      font-weight: 300;
      margin: 0 0 12px;
    }

    .location-section p {
      margin-bottom: 8px;
    }

    .location-buttons {
      margin-top: 18px;
      display: flex;
      gap: 12px;
      flex-wrap: wrap;
    }

    .location-buttons .button {
      background: var(--cream);
      color: var(--green);
      font-size: 16px;
    }

    .location-map img {
      width: 100%;
      height: auto;
      border-radius: 12px;
      object-fit: cover;
    }

    /* CONTACT */
    .contact-section {
      padding: 50px 40px 40px;
      background: var(--cream);
      color: var(--green);
      text-align: center;
    }

    .contact-grid {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 24px;
      margin-bottom: 30px;
    }

    .contact-item h3 {
      font-family: var(--heading-serif);
      font-size: 18px;
      margin-bottom: 6px;
    }

    .contact-item p {
      font-size: 13px;
      margin: 0;
    }

    .contact-logo {
      font-family: var(--heading-serif);
      font-size: 24px;
      margin-top: 10px;
    }

    /* FOOTER */
    footer {
      background: var(--green);
      color: var(--cream);
      padding: 20px 40px;
    }

    .footer-inner {
      max-width: 1200px;
      margin: 0 auto;
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
      gap: 16px;
    }

    .footer-logo {
      font-family: var(--heading-serif);
      font-size: 18px;
    }

    .footer-links {
      display: flex;
      gap: 20px;
      font-size: 13px;
    }

    .footer-links a {
      color: var(--cream);
      text-decoration: none;
    }

    /* RESPONSIVE */
    @media (max-width: 900px) {
      .hero {
        grid-template-columns: 1fr;
      }

      .classes-section .class-grid {
        grid-template-columns: repeat(2, 1fr);
      }

      .about-style {
        grid-template-columns: 1fr;
        text-align: center;
      }

      .about-style p {
        margin: 0 auto 24px;
      }

      .location-section {
        grid-template-columns: 1fr;
      }

      .contact-grid {
        grid-template-columns: repeat(2, 1fr);
      }

      .site-header {
        flex-direction: column;
        gap: 16px;
      }

      .main-nav {
        flex-wrap: wrap;
        justify-content: center;
      }

      .footer-inner {
        flex-direction: column;
        text-align: center;
      }
    }

    @media (max-width: 600px) {
      .classes-section .class-grid {
        grid-template-columns: 1fr;
      }

      .contact-grid {
        grid-template-columns: 1fr;
      }

      .hero,
      .about-style,
      .location-section,
      .classes-section,
      .contact-section {
        padding: 40px 20px;
      }
    }
  </style>
</head>

<body>

  <!-- HEADER -->
  <header class="site-header">
    <a href="#home" class="logo">
      <span>The</span>
      <span>Pilates</span>
      <span>Garden</span>
    </a>

    <nav class="main-nav" aria-label="Main navigation">
      <a href="#home">Home</a>
      <a href="#about">About</a>
      <a href="#classes">Classes</a>
      <a href="#pricing">Membership/Pricing</a>
      <a href="#contact">Contact</a>
      <a href="#booking" class="nav-button">Book Now</a>
    </nav>
  </header>

  <main>

    <!-- HERO -->
    <section class="hero" id="home">
      <div class="hero-content">
        <p class="eyebrow">Mind. Body. Connection.</p>
        <h1>MAT PILATES</h1>
        <p class="hero-subtitle">The Pilates Garden</p>
        <p class="hero-description">
          Outdoor mat Pilates classes designed to help you strengthen your body,
          calm your mind and reconnect with nature.
        </p>
        <a href="#booking" class="button">Book A Class</a>
      </div>

      <div class="hero-image">
        <img src="images/hero-pilates.jpg" alt="Woman practising Pilates in a garden">
      </div>
    </section>

    <!-- CLASSES -->
    <section class="classes-section" id="classes">
      <div class="section-heading">
        <span></span>
        <h2>Classes</h2>
        <span></span>
      </div>

      <div class="class-grid">
        <article class="class-card">
          <img src="images/sculpt.jpg" alt="Sculpt Pilates class">
          <h3>Sculpt</h3>
          <p>Mat Pilates class designed to tone and strengthen.</p>
          <a href="#">Information</a>
        </article>

        <article class="class-card">
          <img src="images/sweat.jpg" alt="Sweat Pilates class">
          <h3>Sweat</h3>
          <p>High intensity Pilates workout for endurance.</p>
          <a href="#">Information</a>
        </article>

        <article class="class-card">
          <img src="images/stretch.jpg" alt="Stretch Pilates class">
          <h3>Stretch</h3>
          <p>Gentle Pilates flow to improve flexibility.</p>
          <a href="#">Information</a>
        </article>

        <article class="class-card">
          <img src="images/sunset.jpg" alt="Sunset Pilates class">
          <h3>Sunset</h3>
          <p>Evening Pilates session to unwind and relax.</p>
          <a href="#">Information</a>
        </article>
      </div>
    </section>

    <!-- ABOUT OUR PILATES STYLE -->
    <section class="about-style" id="about">
      <div>
        <img src="images/about-pilates.jpg" alt="Outdoor Pilates session">
      </div>
      <div>
        <h2>The Pilates Garden</h2>
        <h3>ABOUT OUR PILATES STYLE</h3>
        <p>
          Our mat Pilates style blends mindful movement, breathwork, and the grounding
          energy of nature. Every class is designed to strengthen your body, calm your
          mind, and reconnect you with the outdoors.
        </p>
        <a href="#classes" class="button">Learn More</a>
      </div>
    </section>

    <!-- LOCATION -->
    <section class="location-section" id="location">
      <div>
        <h2>LOCATION</h2>
        <h3>Gold Coast, Australia</h3>
        <p><strong>Address:</strong> 123 Palm Street, Gold Coast, QLD</p>
        <p><strong>Hours:</strong> 6:00am - 7:00pm Mon - Sun</p>
        <div class="location-buttons">
          <a href="#booking" class="button">Book Now</a>
          <a href="#contact" class="button">Learn More</a>
        </div>
      </div>
      <div class="location-map">
        <img src="images/map-goldcoast.jpg" alt="Map showing The Pilates Garden location in Gold Coast">
      </div>
    </section>

    <!-- CONTACT -->
    <section class="contact-section" id="contact">
      <div class="section-heading">
        <span></span>
        <h2>Contact</h2>
        <span></span>
      </div>

      <div class="contact-grid">
        <article class="contact-item">
          <h3>Email</h3>
          <p>Pilates@PilatesGarden.com</p>
        </article>
        <article class="contact-item">
          <h3>Number</h3>
          <p>(123) 456-7890</p>
        </article>
        <article class="contact-item">
          <h3>Location</h3>
          <p>123 Palm Street, Gold Coast, QLD</p>
        </article>
        <article class="contact-item">
          <h3>Instagram</h3>
          <p>@ThePilatesGarden</p>
        </article>
      </div>

      <div class="contact-logo">The Pilates Garden</div>
    </section>

  </main>

  <!-- FOOTER -->
  <footer>
    <div class="footer-inner">
      <div class="footer-logo">The Pilates Garden</div>
      <div class="footer-links">
        <a href="mailto:Pilates@PilatesGarden.com">Email</a>
        <a href="tel:1234567890">Phone</a>
        <a href="#location">Location</a>
        <a href="https://instagram.com/ThePilatesGarden">Instagram</a>
      </div>
    </div>
  </footer>

</body>
</html>
