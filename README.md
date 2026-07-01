# 🌸 Birthday Surprise

A mobile-first, multi-screen birthday website — built as a single static HTML file.

---

## Folder Structure

```
birthday-maluu/
├── index.html          ← The entire site lives here
└── assets/
    ├── photo1.jpg      ← Red background photo (1st date)
    ├── photo2.jpg      ← Video call screenshot
    ├── photo3.jpg      ← Dark / rickshaw photo
    └── music.mp3       ← Background music (plays after first tap)
```

---

## ✏️ Editing Content

**All editable text is in one place** — look for this block near the top of `index.html`:

```html
<!-- ================================================================
     ✏️  EDITABLE CONTENT BLOCK
     All text lives here — change anything below without touching HTML
     ================================================================ -->
<script>
const C = { ... }
</script>
```

Edit only the values inside that `const C = { ... }` object.  
Do **not** touch anything outside those curly braces.

### What you can change:
| Key | What it controls |
|-----|------------------|
| `title` | Browser tab title |
| `opening` | Intro screen text (use `\n` for line breaks) |
| `welcome` | Screen 2 message |
| `heroText` | The "Happy Birthdayy" line |
| `heroName` | The big italic name |
| `subtext` | Subtitle under the name |
| `letterTitle` | Letter screen heading |
| `letter` | Main letter body |
| `signature` | Letter sign-off |
| `memTitle` | Memory gallery heading |
| `photos[n].caption` | Caption under each photo |
| `hlTitle` | Highlights heading |
| `highlights[n].e` | Emoji for each highlight |
| `highlights[n].t` | Text for each highlight |
| `endTitle` | Ending screen title |
| `endMsg` | Final message |

---

## 🚀 Deploying to GitHub Pages

1. Create a new **public** repo on GitHub (e.g. `name-birthday`)
2. Upload the entire `birthday-maluu/` folder contents (not the folder itself — just whats inside)
3. Go to **Settings → Pages**
4. Set source to `main` branch, `/ (root)` folder
5. Hit Save — your URL will be: `https://yourusername.github.io/Birthdayy-wish/`

Share that link with the lucky person 🌸... they should be grateful to have you, I'm sure no one made this for you still you're doing this!

---

## 📱 Experience Flow

1. **Intro** — Tap the 🎀 to unlock the surprise (also triggers music)
2. **Welcome** — A warm hey-there
3. **Birthday** — Big confetti moment with her name
4. **Letter** — A personal note
5. **Memories** — Swipe or tap through 3 photos with captions
6. **Always Remember** — 5 cards that animate in one by one
7. **Ending** — The final sign-off

Music toggle (♪) appears at the top-right from screen 2 onward.  
Music starts after the first tap (required by mobile browsers).  
If music fails to load, the site works fine without it.
