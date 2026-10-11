# Thomas Research Site — starter

A minimal Astro starter matching the research / human-movement visual direction discussed in ChatGPT.

## Open in PyCharm

1. Install Node.js 22.12.0 or newer (Astro 7 requires Node.js 22.12.0+).
2. Unzip this folder somewhere permanent.
3. PyCharm → **File → Open** → select `thomas-research-site`.
4. Open the integrated terminal in PyCharm.
5. Run:

```bash
npm install
npm run dev
```

6. Open the local URL printed in the terminal (normally `http://l---
import '../styles/global-latent-site.css';
import 'bootstrap-icons/font/bootstrap-icons.css';
import { siGooglescholar } from 'simple-icons';
import LatentBackground from "../components/LatentBackground.astro";
import SelectedProjects from "../components/SelectedProjects.astro";
import ResearchApproach from "../components/ResearchApproach.astro";

const projects = [
  {
    number: '01',
    title: 'Structured Latent Spaces for Human Activity Recognition',
    description: 'Can a low-dimensional representation remain both interpretable and operational for activity recognition?',
    tags: ['IMU', 'HAR', 'Representation Learning', 'AAE'],
    type: 'latent'
  },
  {
    number: '02',
    title: 'Motion-Aware Physiological Representations',
    description: 'Using motion information to learn physiological representations that are more robust to movement artifacts.',
    tags: ['PPG', 'IMU', 'Multimodal Learning', 'Digital Health'],
    type: 'signals'
  },
  {
    number: '03',
    title: 'Reduced Representations in Human Activity Recognition',
    description: 'A systematic review of how reduced representations are used, interpreted, and evaluated in HAR research.',
    tags: ['Systematic Review', 'HAR', 'Taxonomy', '153 studies'],
    type: 'review'
  }
];
---
<!doctype html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width" />
    <meta name="description" content="Thomas Rousseau — research on representation learning for human movement, wearable sensing and digital health." />
    <title>Thomas Rousseau — Human Movement Representation Learning</title>

    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />

    <link
      href="https://fonts.googleapis.com/css2?family=Caveat:wght@500;600;700&family=Space+Grotesk:wght@400;500;600;700&family=Space+Mono:wght@400;700&family=Syne:wght@500;600;700;800&display=swap"
      rel="stylesheet"
    />
  </head>
  <body>
    <header class="shell nav">

      <!-- Left: name -->
      <a class="brand" href="#top">
        <strong>Thomas Rousseau</strong>
        <span>PhD Student · The University of Tokyo</span>
      </a>

      <div class="nav-logos">

      <!-- University of Tokyo -->
      <a
        href="https://www2.mech.t.u-tokyo.ac.jp/?lang=en"
        class="nav-logo"
        target="_blank"
        rel="noopener noreferrer"
        aria-label="University of Tokyo Mechanical Engineering"
        title="University of Tokyo"
      >
        <img
          src="/images/ginkgoleaves.jpeg"
          alt="University of Tokyo"
          width="44"
          height="44"
        />
      </a>

      <!-- GVLAB -->
      <a
        href="https://www.gvlab.jp/"
        class="lab-logo"
        target="_blank"
        rel="noopener noreferrer"
        aria-label="Visit GVLAB website"
        title="GVLAB"
      >
        <img
          src="/images/GVLAB.png"
          alt="GVLAB"
        />
      </a>

      </div>

      <!-- Right: navigation -->
      <nav class="nav-links" aria-label="Main navigation">
        <a href="#journey">Journey</a>
        <a href="#research">Research</a>
        <a href="#projects">Projects</a>
        <a href="#publications">Publications</a>
        <a href="#about">About</a>
      </nav>

    </header>

    <main id="top">

      <LatentBackground />

      <section class="shell hero">

        <div>
          <div class="eyebrow">Human movement · Wearable sensing · Representation learning</div>
          <h1>Learning meaningful representations of human movement.</h1>
          <p>
            I develop machine-learning methods to turn wearable sensor data into interpretable representations of human movement.
            My research explores how movement patterns can be recognized, how they evolve with fatigue, and how these representations can support biomechanical and health-related applications.
          </p>
          <div class="actions">
            <a class="btn primary" href="#research">Explore my research ↓</a>
            <a class="btn" href="#projects">View projects →</a>
          </div>
        <div class="socials">

          <!-- GitHub -->
          <a
            href="https://github.com/thomasrss"
            target="_blank"
            rel="noopener noreferrer"
            aria-label="GitHub"
            title="GitHub"
          >
            <i class="bi bi-github" aria-hidden="true"></i>
          </a>

          <!-- CV -->
          <a
            href="/cv/Thomas_Rousseau_CV.pdf"
            target="_blank"
            rel="noopener noreferrer"
            aria-label="View CV"
            title="View CV"
          >
            <i class="bi bi-file-earmark-person" aria-hidden="true"></i>
          </a>

            <a
              href="https://scholar.google.com/citations?user=g6OsxqwAAAAJ&hl=en"
              target="_blank"
              rel="noopener noreferrer"
              aria-label="Google Scholar"
              title="Google Scholar"
            >
              <svg
                viewBox="0 0 24 24"
                width="22"
                height="22"
                fill="currentColor"
                aria-hidden="true"
              >
                <path d={siGooglescholar.path} />
              </svg>
            </a>

          <!-- LinkedIn -->
          <a
            href="https://www.linkedin.com/in/thomas-rousseau31000"
            target="_blank"
            rel="noopener noreferrer"
            aria-label="LinkedIn"
            title="LinkedIn"
          >
            <i class="bi bi-linkedin" aria-hidden="true"></i>
          </a>

          <!-- Email -->
          <a
            href="mailto:thomasrousseau@g.ecc.u-tokyo.ac.jp"
            aria-label="Email"
            title="Email"
          >
            <i class="bi bi-envelope" aria-hidden="true"></i>
          </a>

        </div>
        </div>

        <div class="hero-visual">
          <img
            src="/images/intro.png"
            alt="Human movement data from wearable sensors transformed into a latent representation"
            width="1448"
            height="1086"
          />
        </div>
      </section>

        <!-- =============================
             ACADEMIC JOURNEY
             ============================= -->

        <section class="section academic-path" id="journey">
          <div class="shell">

            <!-- SECTION HEADER -->
            <div class="section-head">
              <div>
                <div class="section-kicker">Academic path</div>
                <h2>My academic journey</h2>
              </div>

              <p>
                From sport science and human movement to biomechanics,
                wearable sensing and representation learning.
              </p>
            </div>


            <!-- TIMELINE + IMAGE -->
            <div class="academic-layout">

              <!-- LEFT : TIMELINE -->
              <div class="academic-timeline">

                <div class="timeline-axis">
                  <div class="timeline-arrow">↑</div>
                </div>


                <!-- PhD -->
                <div class="academic-entry current">

                  <div class="academic-date">
                    <strong>2025</strong>
                    <span>Present</span>
                  </div>

                  <div class="academic-marker"></div>

                  <div class="academic-content">
                    <div class="academic-label">Doctoral degree</div>

                    <h3>PhD Candidate in Mechanical Engineering</h3>

                    <div class="academic-institution">
                      The University of Tokyo · Tokyo, Japan
                    </div>

                    <div class="academic-program">
                      International Multidisciplinary Engineering Program · GVLAB
                    </div>

                    <p>
                      AI-assisted analysis of human movement, fatigue,
                      biomechanics and health-related performance indicators.
                    </p>
                  </div>

                </div>


                <!-- Master of Science -->
                <div class="academic-entry">

                  <div class="academic-date">
                    <strong>2024</strong>
                  </div>

                  <div class="academic-marker"></div>

                  <div class="academic-content">
                    <div class="academic-label">Master of Science</div>

                    <h3>Biomechanics · Biomaterials · Health</h3>

                    <div class="academic-institution">
                      Université de Reims Champagne-Ardenne · Reims, France
                    </div>

                    <div class="academic-honor">
                      Highest Honors · Top of the Class
                    </div>

                    <p>
                      Biomechanics, physiology, neuromotor behavior and
                      quantitative research methods for health applications.
                    </p>
                  </div>

                </div>


                <!-- Master of Education -->
                <div class="academic-entry">

                  <div class="academic-date">
                    <strong>2021</strong>
                  </div>

                  <div class="academic-marker"></div>

                  <div class="academic-content">
                    <div class="academic-label">Master of Education</div>

                    <h3>Physical Education & Sportive Activities</h3>

                    <div class="academic-institution">
                      Université Toulouse II Jean Jaurès · Toulouse, France
                    </div>

                    <div class="academic-honor">
                      Graduated with Honors
                    </div>

                    <p>
                      Pedagogy, human movement and sport science.
                    </p>
                  </div>

                </div>


                <!-- Bachelor -->
                <div class="academic-entry">

                  <div class="academic-date">
                    <strong>2019</strong>
                  </div>

                  <div class="academic-marker"></div>

                  <div class="academic-content">
                    <div class="academic-label">Bachelor's degree</div>

                    <h3>Sports Science & Physical Education</h3>

                    <div class="academic-institution">
                      Université Toulouse III Paul Sabatier · Toulouse, France
                    </div>

                    <div class="academic-honor">
                      Education & Motor Skills · Graduated with Honors
                    </div>

                    <p>
                      Foundation in physiology, motor learning
                      and applied movement science.
                    </p>
                  </div>

                </div>

              </div>
              <!-- END TIMELINE -->


              <!-- RIGHT : ILLUSTRATION -->
              <div class="academic-visual">
                <img
                  src="/images/flow.png"
                  alt="Academic journey from sport science and biomechanics to wearable sensing and representation learning"
                />
              </div>

            </div>
            <!-- END ACADEMIC LAYOUT -->

          </div>
        </section>

      <ResearchApproach />

      <SelectedProjects />

      <section class="section" id="publications">
        <div class="shell">
          <div class="section-head">
            <div><div class="section-kicker">Selected publications</div><h2>Papers</h2></div>
          </div>
          <div class="publications">
            <article class="pub">
              <div class="pub-year">Under review</div>
              <div>
                <div class="pub-title">Reduced Representations in Human Activity Recognition: A Systematic Review and Event-Level Taxonomy</div>
                <div class="pub-authors"><strong>T. Rousseau</strong>, G. Venture, V. Hernandez</div>
                <div class="pub-meta">Systematic review · Human activity recognition · Representation learning</div>
              </div>
              <div class="pub-actions"><a href="#">Under review →</a></div>
            </article>
            <article class="pub">
              <div class="pub-year">2024</div>
              <div>
                <div class="pub-title">Latent space representation of human movement: assessing the effects of fatigue</div>
                <div class="pub-authors"><strong>T. Rousseau</strong>, G. Venture, V. Hernandez</div>
                <div class="pub-meta">IMU & Force plate · Adversarial autoencoders · Operational low-dimensional latent space · Fatigue monitoring · Sport Science</div>
              </div>
              <div class="pub-actions"><a href="https://www.mdpi.com/1424-8220/24/23/7775">Sensors →</a></div>
            </article>
            <article class="pub">
              <div class="pub-year">2024</div>
              <div>
                <div class="pub-title">The measurement of spatiotemporal parameters in running at different velocities: a comparison between a GPS unit and an infrared mat</div>
                <div class="pub-authors">T. Provot, B. Millot, E. Hazotte, <strong>T. Rousseau</strong>, J. Slawinski</div>
                <div class="pub-meta">IMU & Optoeletronic system · Sport Science · Performance indicators · Track and field</div>
              </div>
              <div class="pub-actions"><a href="https://www.mdpi.com/2409-9279/7/6/103">Methods and Protocols →</a></div>
            </article>
          </div>
        </div>
      </section>

      <section class="section soft" id="about">
        <div class="shell about">
          <div class="portrait" aria-label="Photo placeholder">TR</div>
          <div>
            <div class="section-kicker">About me</div>
            <h2 style="font-size:38px;letter-spacing:-.04em;margin:8px 0 12px;">Researching movement through representations.</h2>
            <p>I am a PhD student at The University of Tokyo working on representation learning for human movement, wearable sensing and digital health. My research focuses on making learned representations both useful and interpretable.</p>
            <a class="btn" href="#">More about me →</a>
          </div>
          <div class="about-meta">
            <div><strong>The University of Tokyo</strong>PhD Student</div>
            <div><strong>Research</strong>Movement representations<br/>Wearable sensing<br/>Digital health</div>
            <div><strong>Based in</strong>Tokyo, Japan</div>
          </div>
        </div>
      </section>
    </main>

    <footer class="shell footer">
      <span>© 2026 Thomas Rousseau</span>
      <span>Built with Astro · Replace placeholder links before publishing.</span>
    </footer>
  </body>
</html>

```ocalhost:4321`).

## Main files to edit first

- `src/pages/index.astro` — all homepage content
- `src/styles/global.css` — colors, spacing, typography, layout
- `public/` — later, place your real images / figures here

## Replace these placeholders

- `YOUR_EMAIL`
- GitHub / Scholar / LinkedIn links
- publication status / links
- project links
- `TR` portrait placeholder
- `site` inside `astro.config.mjs`

## Next steps

Once the static homepage is right, split it into Astro components and add dedicated project pages, publication data, real scientific figures, and subtle animations.
