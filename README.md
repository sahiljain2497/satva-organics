# Satva Organics Website

This is a static website for Satva Organics, built with HTML, CSS, and JavaScript. It features a bilingual interface (English/Hindi) and WhatsApp integration for orders.

## Project Structure
- `index.html`: The main landing page.
- `contact.html`: The contact page.
- `styles.css`: All styling, including responsive layouts and animations.
- `script.js`: Handles language toggling, form submissions, and animations.

## How to Edit

### 1. Update Contact Details
To update the Phone Number or WhatsApp Number, you need to edit **two** files:

**In `index.html` and `contact.html` (HTML links):**
- Search for `91XXXXXXXXXX` and replace with your actual 10-digit WhatsApp number (with country code 91).
- Search for `+91XXXXXXXXXX` and replace with your calling number.

**In `script.js` (JavaScript Logic):**
- Look for `const WHATSAPP_NUMBER = "91XXXXXXXXXX";` near the top of the file.
- Replace `91XXXXXXXXXX` with your actual WhatsApp number. This controls where the forms send messages.

### 2. Update Address and Service Areas
- Open `index.html` and `contact.html`.
- Search for "Mohali, Punjab (full address here)" or "Service Areas" to update text.
- If editing text that appears in Hindi as well, you must also update the **Translations** in `script.js`.

### 3. Adding Real Images
Currently, the site uses placeholder colored boxes. To add real images:
1. Create an `images` folder in this directory.
2. Add your images (e.g., `farm.jpg`, `product-5kg.jpg`).
3. In `index.html`, find the `<div class="placeholder-img" ...>` lines.
4. Replace the `<div>` with an `<img>` tag:
   ```html
   <!-- Replace this -->
   <div class="placeholder-img">...</div>

   <!-- With this -->
   <img src="images/farm.jpg" alt="Satva Organics Farm" class="hero-img">
   ```
5. You may need to adjust `styles.css` if the image sizes vary significantly.

### 4. Editing Translations
All translatable text is stored in `script.js` inside the `translations` object.
- `en`: English text
- `hi`: Hindi text

To change a sentence, find the corresponding key (e.g., `hero.subtitle`) and update both the English and Hindi values.

## Deployment
This is a static site. You can host it on:
- GitHub Pages
- Netlify (Drag and drop this folder)
- Vercel
- Any standard web hosting (GoDaddy, Hostinger, etc.) simply by uploading these files to `public_html`.
# satva-organics
