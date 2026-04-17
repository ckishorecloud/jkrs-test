```markdown
# Design System Document: Enterprise Luminescence

## 1. Overview & Creative North Star
**The Creative North Star: "The Sovereign Tech-Vault"**

This design system moves beyond the "standard corporate" aesthetic to establish a visual language of permanence, authority, and futuristic precision. For a firm operating at the intersection of Enterprise IT and Solar Infrastructure in Dubai, the UI must feel as solid as architecture and as fluid as light. 

We break the "template" look by rejecting the rigid 1px border. Instead, we utilize **Asymmetric Spatial Distribution** and **Tonal Layering**. The layout is treated like a curated gallery—expansive white space (The Desert) meeting high-density, high-tech modules (The Infrastructure). Elements should overlap slightly to create a sense of three-dimensional engineering rather than flat web design.

---

## 2. Colors: The Tonal Spectrum
Our palette isn't just a set of colors; it’s a system of light. We rely on the depth of the UAE night sky and the brilliance of the sun.

### Core Palette
- **Primary (#00081E):** Our "Midnight" base. Used for the most significant structural blocks.
- **Secondary (#0042C7):** "Electric Kinetic." To be used for high-momentum interactions and primary CTAs.
- **Tertiary (#755B00 / #C8A74B):** "Liquid Gold." Reserved for premium accents, trust indicators, and "Best-in-Class" solar metrics.

### The Rules of Engagement
*   **The "No-Line" Rule:** 1px solid borders are strictly prohibited for sectioning. Contrast must be achieved through background shifts (e.g., a `surface-container-low` section transitioning into `surface-bright`).
*   **Surface Hierarchy & Nesting:** Treat the UI as stacked sheets of architectural glass. 
    *   *Base:* `background` (#faf9ff)
    *   *Section:* `surface-container-low` (#f1f3ff)
    *   *Component:* `surface-container-lowest` (#ffffff)
*   **The "Glass & Gradient" Rule:** Floating navigation and conversion cards must use Glassmorphism. Apply `surface-container-highest` at 70% opacity with a `24px` backdrop-blur to allow the geometric tech patterns to "ghost" through the UI.
*   **Signature Textures:** Use subtle linear gradients for CTAs: `secondary` (#0042C7) to `secondary_container` (#0056fd) at a 135-degree angle to simulate the shimmer of solar panels.

---

## 3. Typography: The Editorial Authority
We utilize a dual-typeface system to balance technical precision with modern enterprise scale.

*   **Display & Headlines (Manrope):** Chosen for its geometric purity. 
    *   *Usage:* Use `display-lg` (3.5rem) with tight letter-spacing (-0.02em) for hero sections. This conveys a sense of "built" scale.
*   **Body & Labels (Inter):** Chosen for its exceptional legibility in technical IT documentation.
    *   *Usage:* `body-lg` (1rem) for general copy. Ensure a generous line-height (1.6) to provide "breathing room" in complex data sections.

**The Hierarchy Goal:** Typography should feel "Editorial." Headlines should be unapologetically large, while metadata and labels (`label-md`) should be all-caps with increased letter-spacing to mimic engineering blueprints.

---

## 4. Elevation & Depth: Tonal Layering
Traditional drop shadows are too "web-standard." We use atmospheric depth.

*   **The Layering Principle:** Avoid `z-index` shadows. Elevate a card by placing a `surface-container-lowest` card on a `surface-container-low` background. This creates "Natural Lift."
*   **Ambient Shadows:** For "floating" elements like the Sticky Nav or WhatsApp Integration, use: `box-shadow: 0 20px 40px rgba(4, 26, 63, 0.06)`. It must feel like a soft glow, not a dark smudge.
*   **The "Ghost Border":** If a separation is required for accessibility, use the `outline-variant` token (#c5c6cf) at **15% opacity**. It should be felt, not seen.
*   **Glassmorphism:** Use for "Tech Overlays." Semi-transparent containers (`primary_container` at 80% opacity) with backdrop-blur create a high-end, futuristic "Control Center" feel.

---

## 5. Components: Precision Engineered

### Buttons (The Kinetic Drivers)
*   **Primary:** `secondary` background, `on-secondary` text. Rectangular with `DEFAULT` (0.25rem) radius for a "heavy" enterprise feel. No borders.
*   **Tertiary/Gold:** `tertiary_container` background. Use exclusively for "Get a Quote" or "Contact an Expert."

### Cards & Lists (The Knowledge Blocks)
*   **Rule:** Forbid the use of divider lines.
*   **Implementation:** Separate IT service items using `48px` of vertical white space or by alternating background tints between `surface-container-low` and `surface-container-lowest`.
*   **Solar Metrics Card:** Use `surface-container-highest` with a `tertiary` (Gold) accent bar (4px) on the left edge to denote premium status.

### Sticky Navigation
*   **Style:** `surface-container-lowest` at 85% opacity with backdrop-blur. 
*   **Interaction:** On scroll, the container should shrink slightly and the "Ghost Border" (10% opacity) should appear to define the edge against scrolling content.

### WhatsApp Integration & CTAs
*   **Floating Action:** Use a `secondary` circle with a `secondary_fixed_dim` glow. 
*   **Trust Badges:** Rendered in mono-tone `primary_fixed_variant` to ensure they don't distract from the main conversion, but remain authoritative.

---

## 6. Do’s and Don’ts

### Do:
*   **DO** use "Dubai Scale" imagery: High-angle, architectural shots of the city paired with macro shots of solar cells or server blades.
*   **DO** use asymmetric layouts. Align text to the left 1/3 of the screen and high-quality tech imagery to the right 2/3, allowing elements to bleed off-canvas.
*   **DO** treat white space as a luxury. In the UAE market, "spacious" equals "premium."

### Don’t:
*   **DON'T** use standard 1px borders or heavy black shadows. This cheapens the "Enterprise-Grade" promise.
*   **DON'T** use rounded corners above `0.75rem (xl)`. The brand is "Tech-Forward" and "Solid," not "Playful" or "Soft." 
*   **DON'T** clutter the UI. If a section has more than five distinct elements, move to a "Tabbed" or "Layered" navigation style using the Surface Hierarchy.

---
**Director's Note:** This system is not a kit of parts; it is a philosophy of light and structure. Every pixel must feel like it was placed by an architect, not a template. Focus on the tension between the Deep Navy and the Electric Blue—that is where the "IT Energy" lives.```