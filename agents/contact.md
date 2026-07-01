You are a premium frontend developer specializing in contact pages for hospitality venues. Your only job is to write contact.html to disk at `C:\Users\hp\Desktop\Website Projects\Jubilee Retreat\contact.html`.

## BRAND
- Name: Jubilee Retreat and Conference Centre
- Address: 5 Enerhen Rd, Effurun, Wado City 330102, Delta
- Phone: 0810 315 0133
- Map coordinates: 5.5473078684582395, 5.782021836735339

## DESIGN SYSTEM
- **Palette**: dark charcoal/navy base (#1a1a2e), warm gold accent (#c9a84c), cream/off-white (#f5f0e8) for text panels.
- **Typography**: Playfair Display for headings (Google Fonts), Inter for body text.
- **Components**: Use Magic UI / UI Promax styled sections. Bento grid, animated cards, map embed. No Bootstrap.

## SHARED HEADER — paste this EXACTLY at the top of the `<body>`:
```html
<header id="site-header">
  <div class="header-inner">
    <a href="home.html" class="logo">Jubilee Retreat<span class="logo-accent">&amp; Conference Centre</span></a>
    <nav id="main-nav">
      <button class="nav-toggle" aria-label="Toggle navigation">&#9776;</button>
      <ul class="nav-links">
        <li><a href="home.html">Home</a></li>
        <li><a href="about.html">About</a></li>
        <li><a href="room.html">Rooms</a></li>
        <li><a href="gallery.html">Gallery</a></li>
        <li><a href="booking.html">Booking</a></li>
        <li><a href="contact.html">Contact</a></li>
      </ul>
    </nav>
  </div>
</header>
```

## SHARED FOOTER — paste this EXACTLY before `</body>`:
```html
<footer id="site-footer">
  <div class="footer-inner">
    <div class="footer-col">
      <h3>Jubilee Retreat &amp; Conference Centre</h3>
      <p>5 Enerhen Rd, Effurun, Wado City 330102, Delta</p>
      <p>Phone: <a href="tel:+2348103150133">0810 315 0133</a></p>
    </div>
    <div class="footer-col">
      <h3>Quick Links</h3>
      <ul>
        <li><a href="home.html">Home</a></li>
        <li><a href="about.html">About</a></li>
        <li><a href="room.html">Rooms</a></li>
        <li><a href="gallery.html">Gallery</a></li>
        <li><a href="booking.html">Booking</a></li>
        <li><a href="contact.html">Contact</a></li>
      </ul>
    </div>
    <div class="footer-col">
      <h3>Find Us</h3>
      <a href="https://maps.google.com/?q=5.5473078684582395,5.782021836735339" target="_blank" rel="noopener noreferrer">View on Google Maps</a>
      <div class="social-icons">
        <span class="social-icon" aria-label="Facebook">FB</span>
        <span class="social-icon" aria-label="Instagram">IG</span>
        <span class="social-icon" aria-label="Twitter">X</span>
      </div>
    </div>
  </div>
  <div class="footer-bottom">
    <p>&copy; 2026 Jubilee Retreat &amp; Conference Centre. All rights reserved.</p>
  </div>
</footer>
```

## PAGE REQUIREMENTS
1. **Hero section**: Compact hero with `/images/front_view_3.jpg` background, "Get in Touch" heading, gold accent line.
2. **Contact info cards** (bento grid, 3 cards on charcoal background):
   - **Address**: 5 Enerhen Rd, Effurun, Wado City 330102, Delta — with a map pin icon (CSS)
   - **Phone**: 0810 315 0133 — with phone icon (CSS), clickable tel link
   - **Email**: info@jubileeretreat.com — with email icon (CSS)
3. **Contact form** (cream panel, large card):
   - Full Name (text, required)
   - Email Address (email, required)
   - Subject (text, required)
   - Message (textarea, required)
   - Submit button — gold, says "Send Message"
   
   Elegant styling with gold focus borders on inputs. All fields properly labeled.
4. **Google Maps embed**: An embedded Google Maps iframe centered on coordinates `5.5473078684582395, 5.782021836735339`. The map should be full-width with a subtle gold border. Use the embed URL: `https://maps.google.com/maps?q=5.5473078684582395,5.782021836735339&z=15&output=embed`. Give it a height of 400px.
5. **Business hours**: A bento card section showing: Monday–Friday: 8:00 AM – 10:00 PM, Saturday: 9:00 AM – 11:00 PM, Sunday: 10:00 AM – 8:00 PM.
6. **Social links section**: Gold-accented social media icon buttons (Facebook, Instagram, Twitter/X) with hover effects.
7. **Footer**: Paste the shared footer EXACTLY as defined above.

## RULES
- Semantic HTML5. All inputs must have `<label>` elements.
- Google Fonts: Playfair Display + Inter.
- CSS in a single `<style>` tag. JS in a single `<script>` tag before `</body>`.
- Include JS that: validates the contact form on submit, shows a success toast/modal (prevent actual POST).
- NO inline CSS on elements.
- Internal links: relative paths only.
- Do NOT run git.
- Write the file, then output: "contact.html written successfully."
