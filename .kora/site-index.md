# Site index · format 2
Structure and the names of what each page offers. Values that change often — prices, hours, phone,
address — and body copy are deliberately not recorded here; read the page itself for those.

## index.html → /
title: Jamaican Catering in Tampa Bay, FL | Dre's Island Food Services
purpose: Homepage for Dre's Island Food Services, a Jamaican-rooted caterer serving Tampa Bay and Central Florida: service styles, signature dishes, Chef Dre, the Flavor Oasis tasting series, reviews and the catering quote form.
sections:
- `#top` — hero with tagline, quote and menu calls to action, Google rating
- credentials strip: years of experience, guest capacity, training, award nomination
- brand philosophy with two event photos
- `#experiences` "Four ways to bring the island to your table" — service style cards (no prices): Small Bites, Drop-off Feasts, Onsite Family-Style, The Chef's Table
- `#menu` "From Miss Mavis' kitchen to your table" — signature dish plates with one-line descriptions (no prices): Braised Oxtail, Jerk Chicken, Jerk Wings, Curry Goat, Ackee & Saltfish, Jerk Salmon, Jerk Chicken Pasta, Rice & Peas
- `#chef` — chef biography, credentials and portrait: Chef Andre, Miss Mavis, Sandals Resorts, Pasco County EDC
- `#flavor-oasis` — signature tasting-series feature with event artwork, features, latest edition date/venue and event photos: Flavor Oasis, Five-course tasting, Meet the chef, Intimate seating, Live music, Factory 22, Wesley Chapel
- `#process-title` "Effortless from first call to final plate" — three-step booking process and occasion tags: Weddings, Galas, Birthdays, Brunches, Private Dinners, Holiday Parties
- `#gallery-title` "Presentation is part of the flavor" — event photo gallery with captions
- `#reviews` "Five stars, fifteen times over" — three Google review quotes and the aggregate rating: Gillene Nelson, Donyelle Lark-Hill, Madelyn M
- `#faq` "Questions, answered" — FAQ accordion: Where do you cater?, How far in advance should we book?, Can you accommodate dietary restrictions?, Do you cater weddings and large events?
- `#quote` "Let's plan something unforgettable" — catering quote form (name, email, event date, guest count, event type, message) posting to the Kora forms API, contact list, map and directions link
also: The Google rating appears in the hero and again beside the reviews heading.
also: The quote form submit script is inline at the end of index.html, not in assets/site.js.
also: Flavor Oasis edition date and venue are written in the #flavor-oasis section and in llms.txt.

## 404.html → /404
title: Page not found | Dre's Island Food Services
purpose: Platform not-found page (noindex) linking back to the homepage and the phone line.

## support files
Files that are not pages. A line marked [content] holds words or data a visitor reads, so a
change to the site's content can land there; the rest only make the site work or look right.
- `llms.txt` — business summary for AI crawlers: services, dishes, Flavor Oasis, chef, contact: Flavor Oasis, Small Bites, Drop-off Feasts, Onsite Family-Style, Braised oxtail, jerk chicken  [content]
- `robots.txt` — 101 bytes — too small to hold content
- `sitemap.xml` — sitemap listing the homepage (rewritten at deploy)
- `assets/site.js` — header scroll state, mobile menu, scroll reveal and the 404 anchor rewrite

## shared (every page)
The header, navigation, mobile menu and footer are propagated from index.html to every other page by
`shell_propagation`. A change to any of them is made on index.html alone and copied automatically.
