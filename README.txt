ALTA — static website
=====================

FILES
  index.html    the whole site (HTML, CSS, JavaScript, garment artwork)
  images/       put your clothing photos here

PUT IT ONLINE
  Netlify / Vercel   drag this folder onto the dashboard
  GitHub Pages       push the folder, enable Pages on the branch
  cPanel / FTP       upload both items into public_html

  Nothing to install or build. index.html must stay at the top level.

ADD REAL CLOTHING PHOTOS
  1. Save each photo into the images folder, e.g. images/shell-bomber.png
     Use cut-out PNGs with a transparent background, garment on a hanger,
     shot straight on. Flat shots on white will not hang correctly.
  2. Open index.html, find the catalogue (search for: const P=[ ).
  3. On the product you want, change   img:""
     to                                img:"images/shell-bomber.png"
  4. Save. The photo replaces the drawing on the rail, the grid,
     the product page and the bag. Leave img:"" to keep the drawing.

CHANGE THE SHOP
  Brand name   search for ALTA and replace it
  Products     edit the P list (name, price, colour, fabric, description)
  Colours      the :root block at the top of the CSS
