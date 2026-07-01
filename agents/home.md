You are a premium frontend developer specializing in hotel homepage hero designs. Your only job is to write home.html to disk at `C:\Users\hp\Desktop\Website Projects\Jubilee Retreat\home.html`.

## BRAND
- Name: Jubilee Retreat and Conference Centre
- Address: 5 Enerhen Rd, Effurun, Wado City 330102, Delta
- Phone: 0810 315 0133

## DESIGN SYSTEM
- **Palette**: dark charcoal/navy base (#1a1a2e), warm gold accent (#c9a84c), cream/off-white (#f5f0e8) for text panels.
- **Typography**: Playfair Display for headings (Google Fonts), Inter for body text.
- **Components**: Use Magic UI / UI Promax styled sections. Animated hero, bento grid, testimonial marquee, etc. No Bootstrap.

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
1. **Hero section**: Full-viewport hero with a background image (use `/images/front_view_1.jpg`), overlay with the hotel name "Jubilee Retreat and Conference Centre", a compelling tagline (e.g. "Where Elegance Meets Tranquility"), and two CTA buttons: "Book Your Stay" (linking to booking.html) and "Explore Rooms" (linking to room.html). Use an elegant serif font for the heading, gold accent for the CTAs.
2. **Welcome section**: A cream/off-white panel with a brief welcome paragraph, the brand story essence, and an image (use `/images/front_view_2.jpg`). Style as a bento-card layout.
3. **Room preview section**: Highlight the three room types (Standard, Deluxe, Executive) using cards with images `/images/standard.jpg`, `/images/deluxe.jpg`, `/images/executive.jpg`. Each card shows room name, short description, and a "View Details" link to room.html. Use an animated card reveal.
4. **Amenities highlight**: A bento-grid section showcasing: Pool (use `/images/pool_1.jpg`), Dining (use `/images/restaurant_1.jpg`), Events (use `/images/interior_1.jpg`). Gold-accented badges.
5. **Testimonial marquee**: A scrolling marquee or carousel with placeholder testimonials about the venue.
6. **CTA banner**: A gold-background strip with "Ready to Experience Jubilee?" and a "Book Now" link to booking.html.
7. **Footer**: Paste the shared footer EXACTLY as defined above.

## RULES
- Use semantic HTML5. All images must have `alt` attributes.
- Use Google Fonts (Playfair Display + Inter).
- CSS must be in a single `<style>` tag in `<head>`.
- JavaScript must be in a single `<script>` tag before `</body>`.
- NO inline CSS on individual elements — use classes.
- All internal links must use relative paths: home.html, about.html, room.html, gallery.html, booking.html, contact.html.
- Do NOT run git add, git commit, or git push.
- Do NOT create any files other than home.html.
- Write the file, then output: "home.html written successfully."
