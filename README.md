# 🖼️ Easiest-Image-Converter-Resizer

### The World's Easiest Image Converter and Resizer. No installs. No accounts. No "download this 600MB suite to change a file extension."

Your phone took a photo. It's a HEIC or a giant PNG. You just want it as a normal JPEG
so you can text it, post it, or email it without your friend asking "what even is this file."
You don't need Photoshop. You don't need a "free" app that's free until you hit export. You
need a page that opens, does the thing, and gets out of your way.

That's this.

---

## What it does

- 🔄 **Convert** between JPEG, PNG, and WebP
- 📏 **Resize** to a max width/height, so that 12MB phone photo stops being 12MB
- 🎚️ **Quality slider** for JPEG/WebP if you want to fine-tune the size vs. sharpness tradeoff
- 📦 **Batch mode** — drop in a whole folder, convert them all at once
- ⬇️ **Auto-downloads** each result, no gallery to click through
- 🔒 Runs **100% in your browser**. Your photos never get uploaded anywhere. No server ever
  sees them, no "processing" spinner secretly means "uploading," nothing.

Perfect for shrinking phone photos for texting, converting screenshots for a blog post, or
getting a random WebP someone sent you into a format your printer app actually understands.

---

## How to use it

1. Download `image-format-converter.html`
2. Double-click it. Congratulations, that was the installation.
3. Pick your output format (JPEG, PNG, or WebP)
4. Optional: check "Resize images" and set a max dimension if the file is too big
5. Drop your image(s) on the page
6. Hit **Convert & Download**
7. Send it to whoever's been waiting on that photo for twenty minutes

No sign-up. No watermark. No "upgrade to Pro" wall halfway through. No idea what your
pictures even look like, honestly, because they never leave your computer.

---

## Why this exists

Because "I need this photo in a different format and slightly smaller" should not require:
- ❌ Opening a professional editing suite that takes 45 seconds just to boot up
- ❌ Installing a "converter" app that's actually three ad networks wearing a trench coat
- ❌ Paying a monthly subscription to resize a picture of your dog
- ❌ Uploading your personal photos to some random website to find out what happens to them

Your browser can already do all of this. It just needed someone to build the tool that
does exactly the job instead of the tool that does the job plus fourteen upsells.

---

## Good to know

- **HEIC/HEIF (iPhone's default format)** isn't supported as input — browsers can't read it
  natively. If your photos come in as HEIC, switch your iPhone to "Most Compatible" in
  Settings → Camera → Formats, or convert HEIC → JPEG once on your phone first.
- **Animated GIFs** will only convert their first frame — canvas-based conversion can't
  preserve animation. Keep the original if you need the movement.
- **BMP** is supported as input but not offered as an output format, because browsers
  genuinely cannot encode BMP files. PNG is the closest lossless stand-in.
- Resizing keeps the original aspect ratio — no squished photos.

---

## Tech notes (for the curious)

- Pure HTML/CSS/JS, zero build step, zero dependencies
- Uses `<canvas>` to decode, resize, and re-encode images entirely client-side
- JPEG output auto-fills a white background so transparent PNGs don't turn black
- Works offline once the page is saved locally

---

## License

Do whatever you want with it. Go forth and resize. 📸
