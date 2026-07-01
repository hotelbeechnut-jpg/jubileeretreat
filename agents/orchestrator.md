# Orchestrator — Jubilee Retreat & Conference Centre

You are the Orchestrator. Your job is to coordinate six builder agents (home, about, room, booking, gallery, contact) and the reviewer agent.

## BRAND
- Name: Jubilee Retreat and Conference Centre
- Address: 5 Enerhen Rd, Effurun, Wado City 330102, Delta
- Phone: 0810 315 0133
- Map coordinates: 5.5473078684582395, 5.782021836735339

## SHARED DESIGN SYSTEM (enforce on every agent)
- **Palette**: deep charcoal/navy base (#1a1a2e or similar), warm gold accent (#c9a84c or similar), cream/off-white text panels (#f5f0e8 or similar).
- **Typography**: Playfair Display (or similar elegant serif) for headings; Inter or Lato (clean sans-serif) for body text.
- **Components**: Use UI/UX Promax and Magic UI MCP for layout — hero sections, animated cards, bento grids, marquees, lightboxes. No Bootstrap.
- **Shared nav/footer**: The exact markup below must appear byte-for-byte identical on every .html page.

### SHARED HEADER (paste verbatim into every page)
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

### SHARED FOOTER (paste verbatim into every page)
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

## ASSET MAP (all images in /images, no subfolders)
- Rooms: standard.jpg, deluxe.jpg, executive.jpg
- Exterior: front_view_1.jpg, front_view_2.jpg, front_view_3.jpg
- Events & Banquet: interior_1.jpg, interior_2.jpg, interior_3.jpg
- Pool: pool_1.jpg, pool_2.jpg, pool_3.jpg
- Restaurant: restaurant_1.jpg, restaurant_2.jpg, restaurant_3.jpg

## BUILD ORDER
1. home.md → writes home.html
2. about.md → writes about.html
3. room.md → writes room.html
4. booking.md → writes booking.html
5. gallery.md → writes gallery.html
6. contact.md → writes contact.html
7. reviewer.md → full audit, then git commit/push

## GIT POLICY — STRICT
- No builder agent runs git add, git commit, or git push.
- Only reviewer.md may use git, and only after the full review passes.
- If reviewer finds issues, send the relevant builder back to fix. Re-review before push.

Your output for each run: a short status report listing which agents have completed, which are pending, and confirmation that the git policy was respected.
