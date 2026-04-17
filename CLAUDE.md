# Maîtres de la Guitare Manouche

A single-file interactive web app cataloguing the masters of gypsy jazz guitar. Styled in a vintage parchment/sepia aesthetic with gold accents, inspired by the pre-war Parisian world the music comes from.

## File

`gypsy-jazz-guitarists.html` — self-contained HTML/CSS/JS, no build step, no dependencies except Google Fonts.

## What it does

- Displays ~35 guitarist profiles as cards in a responsive grid
- Search by name or nationality
- Filter by era (Founding Era, Post-Django Era, Modern Era, Contemporary Era)
- Click a card to open a modal with the full bio
- Deduplicates entries and sorts alphabetically at runtime

## Data structure

Each guitarist is a JS object in the `guitarists` array:

```js
{
  name: "Django Reinhardt",
  dates: "1910 – 1953",
  nationality: "Belgian-Romani",
  era: "Founding Era",           // controls filter buttons
  tags: ["QHCF", "Improvisation"],
  bio: "Full biographical text…"
}
```

## Eras in use

- Founding Era
- Post-Django Era
- Modern Era
- Contemporary Era

## Design tokens (CSS custom properties)

| Variable | Value | Use |
|---|---|---|
| `--ink` | `#1a0f00` | Primary text |
| `--parchment` | `#f5ead6` | Card backgrounds |
| `--gold` | `#c8972a` | Accents, borders |
| `--rust` | `#8b3a1a` | Era labels |
| `--cream` | `#fdf6e8` | Page background |

## Fonts

Playfair Display · IM Fell English · Cinzel Decorative · Crimson Pro (all via Google Fonts)

## Notable profiles

George Cole and Valentino Cole (Bay Area) are included — George is the project owner. He leads the George Cole Trio (with son Valentino and violinist Anton Patzner), plays with the David Grisman Quintet, and co-founded the Esprit de Django et Stéphane Festival at the Freight and Salvage in Berkeley.
