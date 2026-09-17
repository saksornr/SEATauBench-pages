# SEATauBench project page

A dependency-free research website for **Findings of EMNLP 2026**, inspired by the [SDFT project page](https://self-distillation.github.io/SDFT.html).

## Preview locally

From this directory, run `python3 -m http.server 8000`, then open http://localhost:8000. No build step or package installation is required.

## Publish with GitHub Pages

1. Push this directory to the intended GitHub repository.
2. In **Settings → Pages**, choose **Deploy from a branch**.
3. Select the branch containing the website and the **/ (root)** folder, then save.
4. Open the URL shown by GitHub Pages after deployment completes.

All local URLs are relative, including figure links, so the page supports both an organization site and a repository subpath. `.nojekyll` disables unnecessary Jekyll processing. No custom domain or deployment is configured.

## Editing

- `index.html`: research content, authors, links, metadata, and citation.
- `assets/style.css`: responsive layout and typography.
- `assets/site.js`: clipboard copying with manual-selection fallback.
- `assets/figures/`: locally stored original paper figures.
- `assets/icons/`: the generated 8-bit sitaw icon and browser/home-screen variants.

There are no remote fonts, JavaScript dependencies, analytics, or backend services. Core content remains available with JavaScript disabled. On smaller screens, wide tables scroll within their own container and each figure links to its full-size image.

## Sources and editorial notes

Content and author affiliations were verified against [arXiv:2606.28715v2](https://arxiv.org/abs/2606.28715v2), dated September 5, 2026. The venue label follows the paper's arXiv comments. BibTeX deliberately cites arXiv rather than inventing proceedings metadata.

Figures 2–4 are rendered and cropped from the original PDF, under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). The overview image is the author-provided Figure 1 artwork. Authors: My Chiffon Nguyen, Aulia Adila, Saksorn Ruangtanusak, Kittiphat Leesombatwathana, Vissuta Gunawan Lim, Patomporn Payoungkhamdee, and Samuel Cahyawijaya. Captions on the site are adapted; the plots themselves are unchanged.

The scenario table follows Table 2 and Section 3.1: **S3** is L2 Tool, with English dialogue. The PDF's Figure 2 caption calls L2 Tools “S2”; the website avoids reproducing that inconsistent label. Findings follow Section 5, including the two-agent vs. three-agent qualification and the distinction between quality and robustness. The abstract is split into paragraphs, with resource links shown in the header.

Before publishing, check links, image rendering, mobile layout, keyboard focus, and the Copy BibTeX button. If adding a canonical URL or social preview image, use the actual deployed absolute URL.
