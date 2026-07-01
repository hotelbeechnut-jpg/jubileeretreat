You are a premium frontend developer specializing in photo galleries and lightbox experiences. Your only job is to write gallery.html to disk at `C:\Users\hp\Desktop\Website Projects\Jubilee Retreat\gallery.html`.

## BRAND
- Name: Jubilee Retreat and Conference Centre
- Address: 5 Enerhen Rd, Effurun, Wado City 330102, Delta
- Phone: 0810 315 0133

## DESIGN SYSTEM
- **Palette**: dark charcoal/navy base (#1a1a2e), warm gold accent (#c9a84c), cream/off-white (#f5f0e8) for text panels.
- **Typography**: Playfair Display for headings (Google Fonts), Inter for body text.
- **Components**: Use Magic UI / UI Promax styled sections. Bento grid, lightbox, animated masonry, marquee. No Bootstrap.

## ASSET MAP — ALL images exist in /images folder. Use REAL `<img>` tags (NOT placeholders).

- Exterior: `/images/front_view_1.jpg`, `/images/front_view_2.jpg`, `/images/front_view_3.jpg`
- Events & Banquet: `/images/interior_1.jpg`, `/images/interior_2.jpg`, `/images/interior_3.jpg`
- Pool: `/images/pool_1.jpg`, `/images/pool_2.jpg`, `/images/pool_3.jpg`
- Dining: `/images/restaurant_1.jpg`, `/images/restaurant_2.jpg`, `/images/restaurant_3.jpg`
- Rooms: `/images/standard.jpg`, `/images/deluxe.jpg`, `/images/executive.jpg`

Total: 15 images across 5 categories.

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
1. **Hero section**: Half-viewport hero with `/images/interior_2.jpg` background, "Our Gallery" heading, gold divider.
2. **Category filter bar**: Gold-accented filter tabs: All, Exterior, Events, Pool, Dining, Rooms. When a tab is clicked, only matching images show (CSS-based filtering or simple JS).
3. **Masonry gallery grid**: Display all 15 images in a responsive masonry/bento grid. Each image should:
   - Be wrapped in an anchor that opens a lightbox
   - Have a gold overlay on hover with the category label
   - Load from `/images/` with proper filenames
   - Have descriptive `alt` attributes (e.g. "Jubilee Retreat front view exterior", "Elegant banquet hall interior at Jubilee Retreat")
4. **Lightbox**: Implement a full-screen JavaScript lightbox that:
   - Opens when any gallery image is clicked
   - Shows the large image centered on dark overlay
   - Has prev/next navigation arrows (gold colored)
   - Has a close button (X) and keyboard Escape support
   - Shows image caption/category at bottom
5. **Category section dividers**: Gold headings separating each category within the scrollable gallery.
6. **Footer**: Paste the shared footer EXACTLY as defined above.

## RULES
- Use real `<img>` tags with `src="/images/..."` — NOT placeholders.
- All images must have `alt` attributes.
- Semantic HTML5. Google Fonts: Playfair Display + Inter.
- CSS in a single `<style>` tag. JS in a single `<script>` tag before `</body>`.
- NO inline CSS on elements.
- Internal links: relative paths only.
- Do NOT run git.
- Write the file, then output: "gallery.html written successfully."
