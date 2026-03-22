# kitty-meme 🐾

so i had a folder of like 60+ cat memes sitting on my desktop doing absolutely nothing. this is what happened next.

---

## what is this

a simple gallery site for cat memes. that's it. no backend, no database, no over-engineering.
click a cat, download it, or turn it into your own meme. built in a few evenings because i was bored and cats are funny.

## features (the real ones)

- **browse by mood** — silly / vibes / chaos / sleepy / angry. yes these are real categories
- **search** — type anything into the search bar, it filters live
- **click to open** — lightbox view with a proper download button (actually downloads the file, not just opens it in a new tab)
- **meme maker** — pick any cat from the gallery, slam some text on it, download your masterpiece. classic impact font included, comic sans for the brave
- **hover actions** — hovering a card shows quick save + meme buttons so you don't have to click twice

## stack

literally just HTML, CSS and vanilla JS. no build step. no npm install. no config files. open index.html and it works.

```
kitty-meme/
├── index.html
└── assets/       ← drop your cats here
```

## running it

```bash
git clone https://github.com/yourusername/kitty-meme
cd kitty-meme
# open index.html in a browser, or:
npx serve .
```

that's it. no "npm run dev". no `.env.example`. just a folder and a file.

## adding more cats

drop any `.jpg`, `.png`, or `.gif` into `/assets`, then add an entry to the `images` array in `index.html`:

```js
{ src: "assets/your-cat.jpg", alt: "a brief description", moods: ["silly"] }
// moods can be: silly, vibes, chaos, sleepy, angry (or mix them)
```

## meme maker tips

- font size 40–55 hits the sweet spot for most images
- white text + black stroke is the classic combo
- comic sans font setting is not a joke, it genuinely works for certain cats
- hit "clear text" if you want to start over without reloading the page

## live demo

👉 [kitty-meme-steel.vercel.app](https://kitty-meme-steel.vercel.app/)

---

if you have a really good cat meme that belongs here, open a PR. the bar for quality is "made me exhale from my nose".
