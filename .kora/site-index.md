# Site index · format 2
Structure and the names of what each page offers. Values that change often — prices, hours, phone,
address — and body copy are deliberately not recorded here; read the page itself for those.

## index.html → /
title: Dre's Island Food Services – Island Catering in Wesley Chapel, FL
purpose: Home page for Dre's Island Food Services, showcasing island catering in Wesley Chapel, FL, client work, reviews, and event booking.
sections:
- `#hero` — Hero banner
- `#gallery` — Photo gallery
- `#story` — Company story and service modes: Drop-off, Full service
- `#offerings` "Flavor Oasis" — Event showcase: Flavor Oasis
- `#reviews` "In our clients' words" — Client testimonials: Camille York Adrien, Jean-Luc Adrien, Madelyn M, Donyelle Lark-Hill, Chiquitta Nash
- `#contact` "Tell us about your event." — Contact and booking call to action

## contact-us.html → /contact-us
title: Book Catering | Dre's Island Food Services
purpose: Collect catering event enquiries and contact details for Chef Dre.
sections:
- `#contact` "Tell us about your event" — Catering enquiry form and event booking details: Drop-off, Full service, Factory 22, Wesley Chapel, Florida, Donyelle Lark-Hill
also: The page title, description, and URL appear in both the head tag and the JSON-LD structured data block.

## flavor-oasis.html → /flavor-oasis
title: Flavor Oasis Tasting Event | Dre's Island Food Services
purpose: Showcase Chef Dre's Flavor Oasis tasting event details, experience highlights, and private event booking.
sections:
- `#hero` — Event introduction and primary actions: Flavor Oasis, Chef Dre
- `#offerings` — Event description, edition details, pricing, schedule, and numbered experience highlights: Flavor Oasis, The Second Edition, Factory 22, Discover Exquisite Tastes, A Feast for the Senses, Curated Tasting Stations, Intimate Setting, Meet the Culinary Creator, Entertainment and Ambiance
- `#gallery` "The same care, on every table." — Photo gallery
- `#contact` "Bring the experience to your own event." — Event booking and contact information: Factory 22
also: The event title, description, and event date appear in the visible hero section and in the JSON-LD schema block.

## support files
Files that are not pages. A line marked [content] holds words or data a visitor reads, so a
change to the site's content can land there; the rest only make the site work or look right.
- `llms.txt` — 194 bytes — too small to hold content
- `robots.txt` — 45 bytes — too small to hold content
- `sitemap.xml` — 160 bytes — too small to hold content

## shared (every page)
The header, navigation, mobile menu and footer are propagated from index.html to every other page by
`shell_propagation`. A change to any of them is made on index.html alone and copied automatically.
