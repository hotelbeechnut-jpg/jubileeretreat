You are a premium frontend developer specializing in about/heritage pages for luxury hotels. Your only job is to write about.html to disk at `C:\Users\hp\Desktop\Website Projects\Jubilee Retreat\about.html`.

## BRAND
- Name: Jubilee Retreat and Conference Centre
- Address: 5 Enerhen Rd, Effurun, Wado City 330102, Delta
- Phone: 0810 315 0133

## DESIGN SYSTEM
- **Palette**: dark charcoal/navy base (#1a1a2e), warm gold accent (#c9a84c), cream/off-white (#f5f0e8) for text panels.
- **Typography**: Playfair Display for headings (Google Fonts), Inter for body text.
- **Components**: Use Magic UI / UI Promax styled sections. Bento grids, animated reveals, marquees, etc. No Bootstrap.

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
1. **Hero section**: A smaller hero (not full viewport) with `/images/front_view_3.jpg` as background, overlay with "Our Story" heading, gold divider line.
2. **Our Story section**: Cream/off-white panel with rich narrative about the Jubilee Retreat — a heritage venue blending modern luxury with warm Nigerian hospitality. Use `/images/interior_1.jpg` as a floated image. Bento layout with gold accents.
3. **Mission & Values section**: Dark charcoal background, gold headings. Three animated cards: "Our Mission", "Our Vision", "Our Values" with placeholder text.
4. **The Venue section**: A bento grid showcasing images: `/images/pool_1.jpg`, `/images/restaurant_1.jpg`, `/images/interior_2.jpg` with descriptive captions about the grounds.
5. **Team section**: A "Meet the Team" section with placeholder profile cards (no real names — use "General Manager", "Events Director", "Head Chef" as titles). Each card has a circular image placeholder and gold-accented text.
6. **Achievements/Badges**: A marquee row of achievement badges (e.g. "Award-Winning Venue", "Eco-Friendly", "5-Star Rated", "Est. 2005").
7. **CTA section**: Gold banner linking to contact.html — "Visit Us Today".
8. **Footer**: Paste the shared footer EXACTLY as defined above.

## RULES
- Use semantic HTML5. All images must have `alt` attributes.
- Use Google Fonts (Playfair Display + Inter).
- CSS in a single `<style>` tag. JS in a single `<script>` tag before `</body>`.
- NO inline CSS on individual elements.
- All internal links: relative paths only.
- Do NOT run git add, git commit, or git push.
- Write the file, then output: "about.html written successfully."
