<!-- Design decision for Dre's Island Food Services (PROD). Source: Claude Code homepage concept A - Island Luxe,
     rebuilt as static HTML for Kora (homepage + 404). Concept file: homepage-variants/variant-a-island-luxe.html -->

# DESIGN.md: Dre's Island Food Services

archetype: island-luxe
interaction_level: L2
light_only: true   # owner decision: no dark design / no dark mode

typography:
  display: "Cormorant Garamond"
  body: "Jost"

palette:
  primary: "#1F4A36"
  secondary: "#F8F3EA"
  accent: "#B08D57"
  application: |
    Ivory #F8F3EA ground with paper #FFFDF8 and sand #EFE6D6 bands, ink #1E1C18 text, jungle green #1F4A36 for actions and feature cards, brushed gold #B08D57 for rules and ornaments (gold text uses #7E5F2C for contrast). Cormorant Garamond display (italic green emphasis), Jost body. Light design only, no dark mode. Arched photo frames echo the logo's circle; pill buttons; wide-tracked uppercase eyebrows.

composition: |
  Split hero: serif headline + arched snapper photo with circular inset; credentials strip; philosophy quote with paired photos; four service cards (Chef's Table in green); round-plate signature dishes; sage chef section; numbered process; mosaic gallery; green lead review card; FAQ accordion; quote form card + contact list and map.

content_rules:
  - Hero leads with food (whole red snapper with orchids).
  - Quote-only: never show prices. Four service styles: Small Bites, Drop-off Feasts, Onsite Family-Style, The Chef's Table.
  - Catering only: no jerk-sauce shop section and no link to dresislandflava.com.
  - Flavor Oasis (owner-approved 2026-10-09): signature tasting-series section (#flavor-oasis) built from the Eventbrite listing; 2nd edition Sat Aug 1, 2026, Factory 22 Wesley Chapel. Past event: CTAs ask about the next edition / private tastings.
  - "Chef Dre" throughout; introduced once as Andre "Dre" Christie.
  - Reviews: Gillene Nelson, Donyelle Lark-Hill, Madelyn M. (Google); 5.0 from 15 Google reviews. Trims are marked with an ellipsis.
  - Quote form fields: name*, email*, event date, guest count, event type, message (no package field). Posts to the Kora forms API (form_type catering_quote) with reCAPTCHA v2.
  - Contact: (772) 475-4460, info@dresislandfoodservices.com, 15029 14th St, Dade City, FL 33523, hours "By appointment", Google map embed + directions link.

files:
  - index.html / 404.html share byte-identical kora:shell header/footer blocks.
  - src/input.css holds @theme tokens and the page CSS in @layer components; assets/styles.css is compiled at deploy.
  - assets/site.js: header state, mobile menu, reveal, tabs, mobile action bar, 404 anchor rewrite.
  - All images are local WebP in assets/img (full + -sm 800w); logos are PNG in assets/logo.
