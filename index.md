---
# GitHub Pages homepage — Step 1: name + social links.
# The empty front matter (these --- lines) keeps it working inside your Jekyll repo.
---
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">

  <!-- EDIT: your name (browser tab) -->
  <title>Your Name</title>

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Fraunces:opsz,wght@9..144,500&family=Inter:wght@400;500&display=swap" rel="stylesheet">

  <style>
    :root {
      --bg:     #FDFDFC;
      --ink:    #1C1C1C;
      --muted:  #8A8A8A;   /* default icon color */
      --measure: 42rem;
      --display: 'Fraunces', Georgia, serif;
      --body: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
    }

    * { box-sizing: border-box; }
    body {
      margin: 0; background: var(--bg); color: var(--ink);
      font-family: var(--body); line-height: 1.65;
      -webkit-font-smoothing: antialiased;
    }

    .page { max-width: var(--measure); margin: 0 auto; padding: 6rem 1.5rem 4rem; }

    /* ---- Header: name centered at top ---- */
    header { text-align: center; }

    .name {
      font-family: var(--display); font-weight: 500;
      font-size: 3rem; line-height: 1.05; letter-spacing: -0.01em;
      margin: 0;
    }

    /* ---- Social links row ---- */
    .socials {
      display: flex; justify-content: center; align-items: center;
      gap: 1.6rem; margin-top: 1.6rem;
    }

    .socials a {
      display: inline-flex; color: var(--muted);
      transition: color 0.18s ease, transform 0.18s ease;
    }
    .socials a:hover, .socials a:focus-visible { transform: translateY(-3px); }
    .socials a:focus-visible { outline: 2px solid currentColor; outline-offset: 4px; border-radius: 4px; }

    /* uniform icon size regardless of each SVG's own viewBox */
    .socials svg { width: 26px; height: 26px; display: block; }

    /* brand colors on hover */
    .sc-scholar:hover  { color: #4285F4; }
    .sc-x:hover        { color: #000000; }
    .sc-linkedin:hover { color: #0A66C2; }
    .sc-orcid:hover    { color: #A6CE39; }
  </style>
</head>

<body>
  <main class="page">
    <header>

      <!-- EDIT: your name -->
      <h1 class="name">Your Name</h1>

      <nav class="socials">

        <!-- Google Scholar — EDIT href -->
        <a class="sc-scholar" href="https://scholar.google.com/citations?user=YOUR_ID"
           aria-label="Google Scholar" title="Google Scholar" target="_blank" rel="noopener">
          <svg viewBox="0 0 24 24" aria-hidden="true">
            <path fill="currentColor" d="M5.242 13.769L0 9.5 12 0l12 9.5-5.242 4.269C17.548 11.249 14.978 9.5 12 9.5c-2.977 0-5.548 1.748-6.758 4.269zM12 10a7 7 0 1 0 0 14 7 7 0 0 0 0-14z"/>
          </svg>
        </a>

        <!-- X (Twitter) — EDIT href -->
        <a class="sc-x" href="https://x.com/YOUR_HANDLE"
           aria-label="X" title="X" target="_blank" rel="noopener">
          <svg viewBox="0 0 24 24" aria-hidden="true">
            <path fill="currentColor" d="M18.244 2.25h3.308l-7.227 8.26 8.502 11.24H16.17l-5.214-6.817L4.99 21.75H1.68l7.73-8.835L1.254 2.25H8.08l4.713 6.231zm-1.161 17.52h1.833L7.084 4.126H5.117z"/>
          </svg>
        </a>

        <!-- LinkedIn — EDIT href -->
        <a class="sc-linkedin" href="https://linkedin.com/in/YOUR_HANDLE"
           aria-label="LinkedIn" title="LinkedIn" target="_blank" rel="noopener">
          <svg viewBox="0 0 24 24" aria-hidden="true">
            <path fill="currentColor" d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433a2.062 2.062 0 01-2.063-2.065 2.064 2.064 0 112.063 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/>
          </svg>
        </a>

        <!-- ORCID — EDIT href -->
        <a class="sc-orcid" href="https://orcid.org/0000-0000-0000-0000"
           aria-label="ORCID" title="ORCID" target="_blank" rel="noopener">
          <svg viewBox="0 0 256 256" aria-hidden="true">
            <path fill="currentColor" d="M256 128c0 70.7-57.3 128-128 128S0 198.7 0 128 57.3 0 128 0s128 57.3 128 128z"/>
            <path fill="var(--bg)" d="M86.3 186.2H70.9V79.1h15.4v107.1z"/>
            <path fill="var(--bg)" d="M108.9 79.1h41.6c39.6 0 57 28.3 57 53.6 0 27.5-21.5 53.6-56.8 53.6h-41.8V79.1zm15.4 93.3h24.5c34.9 0 42.9-26.5 42.9-39.7 0-21.5-13.7-39.7-43.7-39.7h-23.7v79.4z"/>
            <path fill="var(--bg)" d="M88.7 56.8c0 5.5-4.5 10.1-10.1 10.1-5.6 0-10.1-4.6-10.1-10.1 0-5.6 4.5-10.1 10.1-10.1 5.5 0 10.1 4.6 10.1 10.1z"/>
          </svg>
        </a>

      </nav>

      <!-- 下一步的内容(简介、研究方向等)会加在这里 -->

    </header>
  </main>
</body>
</html>
