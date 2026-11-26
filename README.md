# Resume-Portfolio

Personal portfolio for Bjay Makara, backend and full-stack developer in Nairobi.
Live at https://gabriel-bjay.github.io/Resume-Portfolio/

The site is drawn as an engineering drawing set: seven numbered sheets with a drawing
register, title blocks, and a detail drawing for the hard part of each project
(REMS, EquiTask, PR Concierge, VHS Video Store). Light mode is a blueline print,
dark mode is a cyanotype, and actions are in red pencil. It also prints as a CV.

It is a single static `index.html` with inline CSS and JS. No framework, no build step.
Fonts are self-hosted in `fonts/` (Archivo, Atkinson Hyperlegible, JetBrains Mono, all
under the SIL Open Font License; licence files are next to them).

See `DESIGN.md` for the visual rules and `PRODUCT.md` for who the site is for.

## Running locally

Serve the folder with any static file server, for example:

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.
