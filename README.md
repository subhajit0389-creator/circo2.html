<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>CircO2 – Nitric Oxide Support for Healthy Circulation & Energy</title>
  <meta name="description" content="CircO2 is a premium nitric oxide support formula designed to help maintain healthy circulation, natural energy, and mental sharpness.">

  <style>
    :root {
      /* Advanced Bionutritionals style palette */
      --dark: #003a70;        /* primary blue */
      --dark2: #00274d;       /* deeper header blue */
      --accent: #d0021b;      /* red CTA button */
      --accent-dark: #a00018; /* darker red hover */
      --bg: #f5f7fa;          /* light grey background */
      --card: #ffffff;
      --text: #333333;
      --muted: #666666;
    }

    * { box-sizing: border-box; }

    body {
      margin: 0;
      font-family: "Segoe UI", Tahoma, sans-serif;
      background: var(--bg);
      color: var(--text);
    }

    a { color: inherit; }

    /* HERO */
    .hero {
      background: linear-gradient(135deg, var(--dark2), var(--dark));
      color: #ffffff;
      padding: 36px 16px 28px;
    }

    .hero-inner {
      max-width: 1120px;
      margin: 0 auto;
      display: grid;
      gap: 20px;
    }

    @media (min-width: 900px) {
      .hero-inner {
        grid-template-columns: minmax(0, 1.1fr) minmax(0, 1fr);
        align-items: center;
      }
    }

    .hero-eyebrow {
      text-transform: uppercase;
      letter-spacing: 2px;
      font-size: 11px;
      opacity: 0.85;
    }

    .hero h1 {
      margin: 16px 0 10px;
      font-size: 32px;
      line-height: 1.2;
    }

    .hero-sub {
      font-size: 17px;
      margin: 0 0 18px;
      opacity: 0.92;
    }

    .hero-cta {
      display: flex;
      flex-direction: column;
      gap: 8px;
      align-items: flex-start;
    }

    .btn-primary {
      display: inline-block;
      padding: 12px 24px;
      background: var(--accent);
      color: #ffffff;
      font-size: 17px;
      text-decoration: none;
      border-radius: 999px;
      font-weight: 600;
      box-shadow: 0 6px 16px rgba(0,0,0,0.3);
      transition: background 0.15s ease, transform 0.15s ease, box-shadow 0.15s ease;
      white-space: nowrap;
    }

    .btn-primary:hover {
      background: var(--accent-dark);
      transform: translateY(-1px);
      box-shadow: 0 9px 22px rgba(0,0,0,0.35);
    }

    .hero-note {
      font-size: 13px;
      opacity: 0.9;
    }

    .hero-badges {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
      margin-top: 10px;
      font-size: 12px;
    }

    .badge {
      border-radius: 999px;
      border: 1px solid rgba(255,255,255,0.45);
      padding: 4px 10px;
      background: rgba(0,0,0,0.08);
    }

    .hero-image img {
      width: 100%;
      max-width: 520px;
      border-radius: 10px;
      border: 1px solid rgba(255,255,255,0.3);
      box-shadow: 0 10px 26px rgba(0,0,0,0.4);
      display: block;
      margin: 0 auto;
    }

    /* GENERIC SECTION */
    .section {
      max-width: 1120px;
      margin: 22px auto;
      padding: 0 16px;
    }

    .section-card {
      background: var(--card);
      border-radius: 12px;
      box-shadow: 0 4px 14px rgba(0,0,0,0.08);
      padding: 22px 18px;
      border: 1px solid #dde3ee;
    }

    .section-title {
      font-size: 24px;
      margin-bottom: 6px;
      color: var(--dark2);
    }

    .section-subtitle {
      font-size: 15px;
      color: var(--muted);
      margin-bottom: 14px;
    }

    .center-cta {
      text-align: center;
      margin-top: 14px;
    }

    /* VIDEO */
    .video-wrapper {
      position: relative;
      padding-top: 56.25%; /* 16:9 */
      border-radius: 10px;
      overflow: hidden;
      background: #000;
      margin-top: 6px;
    }

    .video-wrapper video {
      position: absolute;
      top: 0; left: 0;
      width: 100%;
      height: 100%;
    }

    /* GRID LAYOUTS */
    .grid { display: grid; gap: 16px; }
    @media (min-width: 768px) {
      .grid-2 { grid-template-columns: repeat(2, minmax(0,1fr)); }
      .grid-3 { grid-template-columns: repeat(3, minmax(0,1fr)); }
    }

    /* IMAGE CARD GENERIC */
    .img-card {
      background: #f7f9fc;
      border-radius: 10px;
      padding: 10px;
      text-align: center;
      border: 1px solid #dde3ee;
    }

    .img-card img {
      max-width: 100%;
      border-radius: 8px;
      display: block;
      margin: 0 auto 6px;
    }

    .img-caption {
      font-size: 13px;
      color: var(--muted);
    }

    /* BENEFIT CARDS */
    .benefit-card {
      background: #f9fbff;
      border-radius: 10px;
      padding: 12px 12px 14px;
      border: 1px solid #e1e6f2;
      font-size: 14px;
    }

    .benefit-card strong {
      display: block;
      margin-bottom: 4px;
      color: var(--dark2);
    }

    /* TESTIMONIALS */
    .testimonial-card {
      background: #f9fbff;
      border-radius: 10px;
      border: 1px solid #e1e6f2;
      padding: 10px;
      font-size: 14px;
    }

    .testimonial-card img {
      max-width: 100%;
      border-radius: 8px;
      display: block;
      margin-bottom: 6px;
    }

    /* LIST STEPS */
    .steps-list {
      list-style: none;
      padding: 0;
      margin: 0;
      counter-reset: step;
    }

    .steps-list li {
      counter-increment: step;
      margin-bottom: 10px;
      padding-left: 30px;
      position: relative;
      font-size: 15px;
    }

    .steps-list li::before {
      content: counter(step);
      position: absolute;
      left: 0;
      top: 3px;
      width: 20px;
      height: 20px;
      border-radius: 50%;
      background: var(--dark);
      color: #fff;
      font-size: 12px;
      display: flex;
      align-items: center;
      justify-content: center;
      font-weight: 600;
    }

    /* FAQ */
    .faq-item { margin-bottom: 12px; }

    .faq-q {
      font-weight: 600;
      font-size: 15px;
      margin-bottom: 4px;
      color: var(--dark2);
    }

    .faq-a {
      font-size: 14px;
      color: var(--muted);
    }

    /* FOOTER */
    footer {
      max-width: 1120px;
      margin: 18px auto 70px;
      padding: 0 16px 14px;
      font-size: 12px;
      color: var(--muted);
      text-align: center;
    }

    /* STICKY CTA BAR */
    .sticky-cta {
      position: fixed;
      left: 0;
      right: 0;
      bottom: 0;
      background: #ffffff;
      box-shadow: 0 -2px 10px rgba(0,0,0,0.18);
      padding: 8px 12px;
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 8px;
      z-index: 999;
    }

    .sticky-cta-text {
      font-size: 13px;
      color: var(--dark2);
      display: none;
    }

    .sticky-cta .btn-primary {
      padding: 8px 16px;
      font-size: 15px;
      box-shadow: none;
    }

    @media (min-width: 768px) {
      .sticky-cta-text { display: inline; }
      .sticky-cta {
        justify-content: space-between;
        padding: 8px 24px;
      }
    }
  </style>
</head>

<body>

  <!-- HERO (with top hero image on right) -->
  <header class="hero">
    <div class="hero-inner">
      <div>
        <div class="hero-eyebrow">Nitric Oxide Support • Circulation • Daily Vitality</div>
        <h1>Support Healthy Blood Flow & Natural Energy with CircO2</h1>
        <p class="hero-sub">
          A premium nitric oxide support formula created to help you stay active, energized, and mentally sharp as you age.
        </p>

        <div class="hero-cta">
          <a class="btn-primary" href="https://www.digistore24.com/redir/538695/Sunnyfors/" target="_blank" rel="noopener noreferrer">
            View Official CircO2 Offers
          </a>
          <div class="hero-note">
            Secure ordering on the official Advanced Bionutritionals partner page.
          </div>
          <div class="hero-badges">
            <div class="badge">Science-based nitric oxide support</div>
            <div class="badge">Great-tasting quick-dissolve tablet</div>
            <div class="badge">Designed for healthy circulation & energy</div>
          </div>
        </div>
      </div>

      <div class="hero-image">
        <!-- Hero banner image -->
        <img src="circo2 amazon 1.jpg" alt="CircO2 improves blood flow by 34% in 20 minutes">
      </div>
    </div>
  </header>

  <!-- VIDEO SECTION (near top) -->
  <section class="section">
    <div class="section-card">
      <h2 class="section-title">Watch: How CircO2 Helps Support Healthy Blood Flow</h2>
      <p class="section-subtitle">
        This short video explains how supporting nitric oxide can help you feel more energetic, clear-headed, and active.
      </p>
      <div class="video-wrapper">
        <!-- Make sure this file is in the same folder as circo2.html -->
        <video controls poster="CircO2 3.jpg">
          <source src="CircO2_ Boost Energy.mp4" type="video/mp4" />
          Your browser does not support the video tag.
        </video>
      </div>
      <div class="center-cta">
        <a class="btn-primary" href="https://www.digistore24.com/redir/538695/Sunnyfors/" target="_blank" rel="noopener noreferrer">
          Yes, Show Me the Current Offers
        </a>
      </div>
    </div>
  </section>

  <!-- INGREDIENTS / BENEFITS IMAGE -->
  <section class="section">
    <div class="section-card grid grid-2">
      <div class="img-card">
        <img src="CircO2 1.jpg" alt="CircO2 ingredients and benefits">
        <div class="img-caption">
          Key ingredients include Vitamin C, Vitamin B12, Beet Root Powder, Hawthorn Berry Extract, and L-Citrulline, which are commonly associated with nitric oxide support and overall vascular health.
        </div>
      </div>
      <div class="img-card">
        <img src="CircO2 2.jpg" alt="Support healthy nitric oxide production">
        <div class="img-caption">
          CircO2 is designed to support healthy nitric oxide production, which can play an important role in circulation and energy as part of a healthy lifestyle.
        </div>
      </div>
    </div>
  </section>

  <!-- SUMMARY BENEFITS TEXT + IMAGE -->
  <section class="section">
    <div class="section-card grid grid-2">
      <div>
        <h2 class="section-title">How CircO2 May Support You</h2>
        <p class="section-subtitle">
          Many adults want help maintaining circulation, energy, and stamina as they get older. CircO2 is formulated to support those goals as part of a balanced lifestyle.
        </p>
        <div class="benefit-card">
          <strong>Healthy Circulation</strong>
          Helps support healthy blood flow so oxygen and nutrients can be delivered efficiently throughout the body.
        </div>
        <div class="benefit-card">
          <strong>Everyday Energy</strong>
          Many users report feeling more active and refreshed during the day.
        </div>
        <div class="benefit-card">
          <strong>Active Lifestyle & Stamina</strong>
          Ideal for people who want to stay engaged in walking, exercise, and daily activities.
        </div>
        <div class="benefit-card">
          <strong>Healthy Aging Support</strong>
          Nitric oxide naturally declines with age; CircO2 is designed to help support healthy levels.
        </div>
      </div>
      <div class="img-card">
        <img src="CircO2 5.jpg" alt="CircO2 key benefit summary">
        <div class="img-caption">
          Visual summary of potential benefits when CircO2 is used regularly alongside a healthy lifestyle. Individual experiences vary.
        </div>
      </div>
    </div>
  </section>

  <!-- GRAPH + ATHLETE IMAGE -->
  <section class="section">
    <div class="section-card grid grid-2">
      <div class="img-card">
        <img src="CircO2 – 9.png" alt="Nitric oxide levels graph">
        <div class="img-caption">
          Example representation of nitric oxide support over time with regular use as described by the manufacturer. Results are individual and may vary.
        </div>
      </div>
      <div class="img-card">
        <img src="CircO2 3.jpg" alt="Athletic performance benefits visual">
        <div class="img-caption">
          CircO2 is often promoted to support stamina, endurance and recovery as part of an overall fitness routine.
        </div>
      </div>
    </div>
  </section>

  <!-- SUPPLEMENT FACTS + TRUST BADGES -->
  <section class="section">
    <div class="section-card grid grid-2">
      <div class="img-card">
        <img src="CircO2 – 11.png" alt="CircO2 supplement facts">
        <div class="img-caption">
          Supplement facts panel as provided by the manufacturer. Always review the label on the product you receive for the most current information.
        </div>
      </div>
      <div class="img-card">
        <img src="CircO2  4.png" alt="Supplement facts with badges">
        <div class="img-caption">
          Visual emphasizing additional attributes such as gluten-free, non-GMO, and other quality indicators as highlighted by the brand.
        </div>
      </div>
    </div>
  </section>

  <!-- HOW TO USE -->
  <section class="section">
    <div class="section-card grid grid-2">
      <div>
        <h2 class="section-title">How to Use CircO2</h2>
        <p class="section-subtitle">
          Always follow the directions on the product label and consult your healthcare provider before starting any supplement.
        </p>
        <ul class="steps-list">
          <li>Place one tablet on your tongue and allow it to dissolve completely.</li>
          <li>Use as directed on the label (often one tablet in the morning and one later in the day initially).</li>
          <li>After the first phase, follow the maintenance schedule recommended on the label.</li>
        </ul>
        <p style="font-size: 13px; color: var(--muted); margin-top: 10px;">
          This summary is for general educational purposes and does not replace medical advice. Always read and follow the label.
        </p>
      </div>
      <div class="img-card">
        <img src="CircO2 – 8.png" alt="How to use CircO2 visual">
        <div class="img-caption">
          Example illustration of how to use CircO2 quick-dissolve tablets as presented in the brand’s materials.
        </div>
      </div>
    </div>
  </section>

  <!-- STRONG BENEFITS PANEL -->
  <section class="section">
    <div class="section-card grid grid-2">
      <div class="img-card">
        <img src="CircO2 – 10.png" alt="Exercise performance benefits visual">
        <div class="img-caption">
          Marketing imagery describing how CircO2 is positioned for blood flow, performance and recovery support. Statements are provided by the brand; your results may vary.
        </div>
      </div>
      <div class="img-card">
        <img src="CircO2 4.png" alt="Key benefits summary panel">
        <div class="img-caption">
          Additional summary of how the product is promoted for circulation, performance, and recovery support.
        </div>
      </div>
    </div>
  </section>

  <!-- KEN H TESTIMONIAL -->
  <section class="section">
    <div class="section-card">
      <h2 class="section-title">What Some Customers Report</h2>
      <p class="section-subtitle">
        Individual experiences are different, but many customers share positive feedback about their energy, circulation support and overall vitality.
      </p>
      <div class="testimonial-card">
        <img src="CircO2 7.jpg" alt="Ken H testimonial">
        <p style="margin-top: 6px;">
          This image reflects one of the testimonial styles used in CircO2 marketing materials. Experiences like feeling “better than I have in 10 years” are individual and are not guaranteed results.
        </p>
      </div>
      <div class="center-cta">
        <a class="btn-primary" href="https://www.digistore24.com/redir/538695/Sunnyfors/" target="_blank" rel="noopener noreferrer">
          Go to Official CircO2 Offer Page
        </a>
      </div>
    </div>
  </section>

  <!-- FAQ -->
  <section class="section">
    <div class="section-card">
      <h2 class="section-title">Frequently Asked Questions</h2>

      <div class="faq-item">
        <div class="faq-q">Is CircO2 a medicine?</div>
        <div class="faq-a">
          No. CircO2 is a dietary supplement designed to support healthy nitric oxide levels, circulation, and energy as part of a balanced lifestyle.
          It is not intended to diagnose, treat, cure, or prevent any disease.
        </div>
      </div>

      <div class="faq-item">
        <div class="faq-q">How soon might I notice a difference?</div>
        <div class="faq-a">
          Experiences vary. Some people feel a difference in their daily energy and circulation support within days or weeks,
          while for others it may take longer. Consistent use as directed is important.
        </div>
      </div>

      <div class="faq-item">
        <div class="faq-q">Can I take CircO2 with my medications?</div>
        <div class="faq-a">
          Always speak with your doctor or healthcare provider before taking any supplement, especially if you have medical conditions
          or are currently taking medications.
        </div>
      </div>

      <div class="faq-item">
        <div class="faq-q">Where do I order the genuine product?</div>
        <div class="faq-a">
          For the authentic CircO2 formula and current offers, order only through the official page linked from this site.
        </div>
      </div>

      <div class="center-cta">
        <a class="btn-primary" href="https://www.digistore24.com/redir/538695/Sunnyfors/" target="_blank" rel="noopener noreferrer">
          Visit Official CircO2 Website
        </a>
      </div>
    </div>
  </section>

  <!-- FOOTER -->
  <footer>
    This independent promotional page is for informational and marketing purposes only and does not provide medical advice.
    Results and experiences vary from person to person. Always read the full product label and consult your healthcare provider
    before using any dietary supplement.
  </footer>

  <!-- STICKY CTA BAR -->
  <div class="sticky-cta">
    <span class="sticky-cta-text">Ready to support your circulation and daily energy with CircO2?</span>
    <a class="btn-primary" href="https://www.digistore24.com/redir/538695/Sunnyfors/" target="_blank" rel="noopener noreferrer">
      Order CircO2 Now
    </a>
  </div>

</body>
</html>
