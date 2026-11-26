# Design: an engineering drawing set

The page is a set of drawings. Keep every new piece inside that idea.

## Colour
| Token | Light (blueline print) | Dark (cyanotype) | Use |
|---|---|---|---|
| `--paper` | `#F2F5F8` | `#11325E` | page and sheet background |
| `--line` | `#1F4E8C` | `#E9F0F8` | frames, rules, figures |
| `--line-soft` | `#9DB3CF` | `#5E7FA8` | minor rules, grid |
| `--ink` | `#102340` | `#E9F0F8` | body text |
| `--ink-soft` | `#4A5E78` | `#B3C6DD` | secondary text, labels |
| `--pencil` | `#C2352B` | `#FF8A7A` | actions and corrections only |
| `--ok` | `#1F6E4A` | `#8FE0B5` | success states, live dots |

Red pencil is for things you can click and for "this is wrong" marks. Never use it as decoration.

## Type
- **Archivo** 800 for headings, 600 for small headings.
- **Atkinson Hyperlegible** for body text.
- **JetBrains Mono** for labels, title blocks, figures and code, with ligatures off.
- Labels are mono, uppercase, letter-spaced, 0.75rem.

## Parts
- **Sheet:** a 1.5px frame with registration ticks on two corners and a title block on top
  (sheet number, name, scale, revision). Scale and revision hide on phones.
- **Drawing register:** the table of contents on sheet 01.
- **Detail:** a framed box with a circled letter (A, B, C, D) for the hard part of a project.
- **Figures:** inline SVG with lines in `--line`, leader lines to labels, and red dashes for
  the wrong or rejected path. Text is at least 13px in the viewBox, and figures are at most
  372 units wide so labels stay readable on a 375px phone.
- **Buttons:** square, 1.5px red-pencil border, filled on hover. No arrows, triangles or icons
  except the green live dot.

## Motion
Only Detail A moves: it plays once when it scrolls into view and has a Replay button.
With reduced motion, or without JavaScript, it shows the final state.

## Must keep
Dark mode (system setting plus the toggle), the sticky bar with its progress line,
back-to-top, copy buttons on code, print-as-CV, no sideways scroll at 375px.
