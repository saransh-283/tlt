# The Leadership Thread – Create Your Profile

Built with semantic HTML and modular CSS (no JavaScript). Deployed via GitHub Pages.

## Hosted URL

- Live site: https://saransh-283.github.io/tlt/

## Codebase overview

- `index.html` — Page structure and form markup.
- `css/` — Styles, split by responsibility:
  - `universal.css` — Design tokens (`:root` variables) and global base (reset, layout header/brand/user-info).
  - `form.css` — Form section layout, grids, headings, labels.
  - `controls.css` — Inputs, textarea, placeholders, focus ring.
  - `dropdown.css` — Custom dropdown component styles.
  - `mappings/` — Mappings between selected radio values and visible dropdown label:
    - `role.css`
    - `specialty.css`
    - `location1.css`
    - `location2.css`.
  - `checkbox.css` — Checkbox styling.
  - `actions.css` — Buttons and action row.
  - `devices/desktop.css`, `devices/mobile.css` — Device-specific tweaks via media queries.
- `assets/` — Images and screenshots.
  - `assets/images/` — Logos and avatars.
  - `assets/screenshots/` — UI screenshots for docs.

### Design tokens

- Font sizes: `--text-sm`, `--text-2xl`
- Font weights: `--font-normal`, `--font-medium`, `--font-semibold`
- Colors: `--color-primary`, `--color-secondary`, `--color-surface`, `--color-text`, `--color-white`, `--color-muted`, etc.
- Spacing scale: `--space-sm`, `--space-md`, `--space-lg`, `--space-xl`, `--space-2xl`, `--space-5xl`
- Shapes/sizes: `--radius-md`, `--h-10`

## Workflow

- No build step. Open `index.html` directly in a browser, or serve locally.
- Edit tokens in `css/universal.css` to theme colors/spacing/typography.
- Component styles live in separate files under `css/` for clarity and reuse.
- Custom dropdowns are CSS-only; radios submit real values, and the selected label is reflected via `:has()` + CSS variables.


## Deployment

- Hosted with GitHub Pages at the URL above.