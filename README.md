# 🎁 The Soloist | Secret Santa Gift Page

A premium, interactive QR-scannable gift reveal experience for a succulent plant personalized as a band member.

## ✨ Features

- **QR-Scannable Design** – Opens directly from phone camera, no app needed
- **Gift Card Reveal Overlay** – Elegant initial screen before reveal
- **Hero Video Section** – Autoplaying succulent video with glassmorphic badge
- **Seasonal Sparkle Confetti** – 100 falling emoji sparkles (🎄✨❄️⭐) on reveal
- **Premium Animations** – Smooth transitions, staggered text reveals, floating effects
- **Background Depth** – Radial gradient lighting with subtle vignette
- **Personalization** – Custom desk reference ("Now performing live at Srini's desk")
- **Care Guide** – Styled "tour rider" with planting instructions
- **Background Music** – Soft ukulele track plays on reveal (with fallback)
- **Mobile Optimized** – Fully responsive, tested on iPhone and Android
- **Office-Safe** – No autoplay noise, calm aesthetic, professional typography

## 📁 Files Included

```
index.html      Main page (HTML + CSS + JavaScript)
hero.mp4        Succulent plant video (autoplay on reveal)
music.mp3       Ukulele background track (plays on button click)
README.md       This file
```

## 🚀 How to Use

### Local Testing
```bash
# Navigate to project folder
cd "path/to/Secret Santa"

# Start local server
python -m http.server 8000

# Open in browser
http://localhost:8000
```

### Deploy to Web
Choose one of these free options:

**GitHub Pages:**
1. Create a GitHub repository
2. Push these 3 files to `main` branch
3. Enable Pages in repo settings (source: main)
4. Access at `https://yourusername.github.io/repo-name`

**Netlify:**
1. Visit netlify.com
2. Drag & drop folder with 3 files
3. Deploy instantly
4. Get shareable URL

**Vercel:**
1. Visit vercel.com
2. Import project
3. Deploy in one click
4. Automatic deployment on push

### Generate QR Code
Once deployed:
1. Copy the live URL (e.g., https://your-site.com)
2. Visit [qr-code-generator.com](https://www.qr-code-generator.com)
3. Paste URL, generate code
4. Download and print
5. Attach to plant pot with label "Scan me 👀"

## 🎨 Customization

### Change Recipient Name
Find this line in `index.html`:
```html
<p class="desk-line">Now performing live at Srini's desk 🌱🎸</p>
```
Replace `Srini` with the recipient's name.

### Update Care Instructions
Find the care guide table:
```html
<tr><td><b>🌥️ Stage Light</b></td><td>Indirect spotlight (Bright room)</td></tr>
<tr><td><b>💧 Hydration</b></td><td>Every 2-3 weeks (Performance fee)</td></tr>
<tr><td><b>🎧 Vibe</b></td><td>Responds well to lo-fi beats</td></tr>
```
Edit the text in `<td>` tags as needed.

### Change Colors
Edit CSS variables at the top of `<style>`:
```css
:root {
    --cream: #FDFBF7;           /* Background */
    --warm-tan: #E8DFD5;        /* Accents */
    --guitar-orange: #E67E22;   /* Buttons, highlights */
    --sage: #7D8C71;            /* Text, dividers */
}
```

### Adjust Confetti Count
Find this line in the `createConfetti()` function:
```javascript
for (let i = 0; i < 100; i++) {
```
Change `100` to any number (30-150 recommended).

### Swap Music/Video
Replace these files in the folder:
- `hero.mp4` – Any short plant/nature video (mute + loop)
- `music.mp3` – Any 30-60 second instrumental track

No code changes needed if names stay the same.

## 🌐 Browser Compatibility

| Browser | Desktop | Mobile |
|---------|---------|--------|
| Chrome  | ✅      | ✅     |
| Safari  | ✅      | ✅     |
| Firefox | ✅      | ✅     |
| Edge    | ✅      | ✅     |

**Requirements:**
- Modern browser (ES6 support)
- Video: MP4 codec H.264
- Audio: MP3 codec
- CSS: Gradient, animation, backdrop-filter support

## 🎯 Experience Flow

1. **Scan QR Code** → Mobile browser opens page
2. **Gift Card Overlay** → See bouncing gift emoji
3. **Click "Reveal"** → Overlay fades, scroll jumps to top
4. **Page Slides In** → Content animates from top
5. **Hero Appears** → Video plays with floating badge
6. **100 Sparkles Fall** → Confetti moment
7. **Music Plays** → Soft ukulele in background
8. **Read Content** → Care guide, personalization, signature
9. **Optional** → Click music button to replay song

## 💡 Pro Tips

- **Video** – Keep under 5MB for fast loading. Muted for browser autoplay policy.
- **Music** – Plays on reveal only (no autoplay disruption). Manual button available.
- **Mobile** – Test on actual device before gifting. Portrait orientation works best.
- **Timing** – Deliver during work day when recipient can enjoy privately.
- **Presentation** – Print QR code on paper or sticker for physical reveal moment.

## 📝 License

Free to use, modify, and share. Made with ❤️ for thoughtful gifting.

## 🎵 Credits

- **Font** – Crimson Pro (Google Fonts)
- **Music** – Bensound Ukulele (CC license)
- **Design Inspiration** – Premium SaaS aesthetics (Notion, Apple, Figma)
- **Built With** – HTML5, CSS3, Vanilla JavaScript (no dependencies)

---

**Questions or improvements?** This project is designed to be simple and hackable. Feel free to customize freely.

Happy gifting! 🎁✨
