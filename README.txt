ACADEMIC RESEARCH WEBSITE — VERSION 3
=====================================

WHAT'S NEW
----------
- Fully designed research overview with five clickable projects.
- Five dedicated research pages with introduction, background, research
  questions, methods, project notes, illustrative SVG and figure placeholders.
- Homepage links updated to navigate to the research subpages.
- Responsive design extends the existing minimalist white / navy style.
- All research diagrams are conceptual illustrations, not actual results.
- No invented publication or personal-profile links.

HOW TO VIEW THE COMPLETE SITE
-----------------------------
1. EXTRACT the entire ZIP archive. Do not open HTML files inside the ZIP.
2. Open index.html from inside the extracted website folder.
3. Click Research in the top navigation or any of the five research cards.

IMPORTANT: Preserve the directory structure so CSS, illustrations, and
internal links resolve correctly:

academic-research-website-v3/
  index.html
  index-standalone.html
  research/
    index.html
    exoplanet-dynamics.html
    galactic-dynamics.html
    asteroseismology.html
    tambo-detectors.html
    fractals-dynamical-systems.html
  assets/
    css/style.css
    illustrations/*.svg
    documents/ (place your CV here later)

The index-standalone.html homepage contains embedded CSS and can be opened
alone. For project links and project pages, keep the whole folder together.
The modular pages use relative stylesheet paths:
  homepage: assets/css/style.css
  research: ../assets/css/style.css

ADDING YOUR ACTUAL RESULTS
--------------------------
Each research page includes a section "Figures & research outputs" with a
placeholder. To replace it:
- Place a figure in assets/images/ (e.g. exoplanet-resonance.png).
- On the project's HTML page, replace the div with class figure-placeholder:
  <figure class="research-figure">
    <img src="../assets/images/exoplanet-resonance.png"
         alt="Descriptive scientific figure alt text">
    <figcaption>Your scientific caption here.</figcaption>
  </figure>
- The figures already have default responsive CSS rules (below).

PERSONAL INFO
-------------
Your Name / YN, LinkedIn URL, ORCID ID, and CV PDF are placeholders.
The TAMBO and fractal project pages intentionally avoid asserting specific
individual results or detector duties that have not yet been provided.
The TAMBO experiment concept can be reviewed here:
  https://investigacion.pucp.edu.pe/grupos/hep/proyecto/tambo/

EDITING
-------
Change colors and layout centrally in assets/css/style.css.
The standalone homepage is a frozen CSS snapshot; if styles change,
regenerate the standalone HTML by embedding updated CSS.
