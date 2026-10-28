# Architecture — UM Publishers Website

## Overview
The project is a static, multi-page website. Each page is a standalone HTML document and shares one external stylesheet. There is no server-side code, data layer, JavaScript, or build pipeline.

## Page responsibilities
- `index.html`: brand introduction, featured fictional books, services overview, value proposition, process preview, sample testimonials, and primary calls to action.
- `about.html`: mission, vision, values, and author-first approach.
- `services.html`: nine service cards with links to enquiry.
- `publishing.html`: staged overview of manuscript preparation, editorial work, design, formats, distribution, and rights considerations.
- `marketing.html`: launch planning, visibility, author branding, campaign planning, and audience building.
- `portfolio.html`: ten fictional titles with locally stored original SVG cover graphics.
- `packages.html`: three illustrative packages and scope caveats.
- `process.html`: five-step publishing workflow.
- `faq.html`: native HTML `details` and `summary` expandable questions; no scripting is needed.
- `contact.html`: accessible demonstration enquiry form. The form is not connected to a service and does not send or persist data.

## Shared styling
`css/style.css` centralizes the navy/orange palette, typography, spacing, buttons, cards, header/footer, responsive grids, focus styles, and animations. Shared HTML fragments are repeated across pages to keep the project simple to understand and edit without a templating tool.

## Assets
`assets/images/` contains original SVG assets authored for this project: ten book covers, one hero illustration, and one favicon. SVG keeps the package small and artwork crisp at different screen sizes. All paths are relative to each HTML file so local browsing and static hosting work without external asset services.

## Responsive approach
CSS Grid and Flexbox create flexible layouts. Media queries at 1050px, 780px, and 520px adjust navigation, cards, forms, book covers, and footer columns. A checkbox and label expose the mobile navigation without JavaScript. Images scale within their containers to avoid horizontal overflow.

## CSS-only motion and accessibility
Hover transitions lift cards and emphasize links. A brief keyframe entrance effect and subtle hero badge drift add motion. The `prefers-reduced-motion: reduce` query minimizes animation for visitors who prefer reduced motion. Semantic landmarks, a skip link, meaningful image alternative text, visible keyboard focus, labels associated with form controls, and native details/summary improve usability.

## Why no JavaScript or backend is needed
The assignment requires a static frontend. Navigation, responsive layouts, hover effects, animations, and expandable FAQs are supported by HTML and CSS. A live enquiry form would require a backend or form service, so this implementation intentionally leaves it as a demonstration-only form and does not claim to transmit data.
