---
title: "About me"
type: "about"
---

<div class="about-pro">

  <!-- HERO / INTRO CARD -->
  <section class="about-hero">
    <div class="about-hero-inner">
      <h1 class="about-title">About me</h1>
      <p class="about-subtitle"> Independent,versatile consultant based in Amsterdam.</p>
    </div>
  </section>

  <!-- MAIN GRID -->
  <section class="about-grid">

    <!-- LEFT COLUMN -->
    <div class="about-left">

      <div class="about-card">
        <h2>What I do</h2>
        <p>
          My name is Sophia Zhukovsky. I'm a freelance professional with over six years of experience in project management,
          research, operations, and administrative support.
        </p>
      </div>

      <div class="about-card">
        <h2>Background</h2>

        <p>
          After earning my BA in Political Science in my home state of New York, I decided it was time to engage with the
          world at an even greater level. I moved to the Netherlands to complete an MSc in Global Environmental Change and
          Policy, and I'm now priviliged to call Amsterdam my home base.
        </p>

        <p>
          Over the years, I've worked in climate tech, UN-affiliated nonprofits, and community centric-spaces. I've co-developed
          and delivered large-scale conferences, designed climate tech pilots, and supported EU grant applications. No two
          experiences have been alike, and the adaptability I've gained through the process is exactly my superpower.
        </p>

        <p>
          I care deeply about sustainability, because to me, it means more than buzzwords or frameworks. It means building an
          organization or initiative that contributes to its community, advancing causes from social equity to environmental
          protection. I'm deeply passionate about using my versatile skillset to help you achieve outcomes that matter.
        </p>
      </div>

      <div class="about-card about-cta">
        <p class="about-cta-text">
          Get in touch today to discuss your needs, and how my services can meet them.
        </p>
      </div>

    </div>

    <!-- RIGHT COLUMN -->
    <div class="about-right">

      <div class="about-card">
        <h2>Where I work</h2>
        <div class="about-gallery">
          {{< gallery dir="gallery" >}}
        </div>
      </div>

      <div class="about-card">
        <!-- keep your existing figure -->
        {{< figure src="/img/about/about-gallery/about-gallery-1.jpg" >}}
      </div>

    </div>

  </section>

</div>

<style>
/* --- Page wrapper --- */
.about-pro{
  max-width: 1180px;
  margin: 0 auto;
  padding: 32px 20px 70px;
  font-family: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial;
}

/* --- Hero --- */
.about-hero{
  margin-bottom: 26px;
}
.about-hero-inner{
  padding: 26px 26px;
  border-radius: 22px;
  background: rgba(0,0,0,.02);
  border: 1px solid rgba(0,0,0,.06);
}
.about-title{
  margin: 0 0 6px;
  font-size: 44px;
  letter-spacing: -0.02em;
}
.about-subtitle{
  margin: 0;
  font-size: 18px;
  opacity: .8;
  line-height: 1.6;
}

/* --- Grid layout --- */
.about-grid{
  display: grid;
  grid-template-columns: 1.1fr .9fr;
  gap: 28px;
  align-items: start;
}
@media (max-width: 980px){
  .about-grid{ grid-template-columns: 1fr; }
}

/* --- Cards --- */
.about-card{
  background: #fff;
  border: 1px solid rgba(0,0,0,.08);
  border-radius: 22px;
  padding: 22px 22px;
  box-shadow: 0 14px 35px rgba(0,0,0,.08);
  margin-bottom: 18px;
}

.about-card h2{
  margin: 0 0 12px;
  font-size: 22px;
  letter-spacing: -0.01em;
}

.about-card p{
  margin: 0 0 14px;
  line-height: 1.75;
  font-size: 16.5px;
  opacity: .92;
}
.about-card p:last-child{ margin-bottom: 0; }

/* --- Gallery section tweaks --- */
.about-gallery{
  margin-top: 12px;
}

/* Hover “pop” for images */
.about-card img{
  border-radius: 18px;
  transition: transform 180ms ease, box-shadow 180ms ease;
  box-shadow: 0 10px 26px rgba(0,0,0,.10);
}
.about-card img:hover{
  transform: translateY(-6px);
  box-shadow: 0 18px 40px rgba(0,0,0,.16);
}

/* CTA block */
.about-cta{
  border-style: dashed;
}
.about-cta-text{
  font-size: 17px;
  margin: 0;
}

/* Reduce motion */
@media (prefers-reduced-motion: reduce){
  .about-card img{ transition: none; }
}
</style>