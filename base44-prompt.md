# Base44 Build Prompt — DragonDoner Brand Playbook

Build a cinematic one-page brand website + mini playbook for **DragonDoner**, a Berlin street-food brand that fuses the original Berlin döner kebab (invented 1972) with Korean kimchi and dragon fire. Domain brand: dragondoner.com. Tone: loud, warm, editorial, night-market cinematic.

## Assets (upload these files into the app's file/asset manager, keep exact paths)

```
/assets
  hero.jpg        — hero: kimchi döner wrapped in a flame dragon, Berlin TV tower behind (2048×1152)
  origin.jpg      — 1970s West Berlin Imbiss döner spit, "DÖNER 2,- DM" sign (1024×1536)
  ingredients.jpg — fine-cut vegetables + kimchi flat-lay (1536×1024)
  breads.jpg      — three breads (pide quarter, dürüm, sesame roll) + three sauces (1536×1024)
  people.jpg      — diverse friends eating DragonDoner at a neon-lit Berlin stand (2048×1152)
  story.mp4       — 8s brand film, 16:9: dragon flames coil around the döner, TV tower bokeh
/social
  logo.png        — transparent logo mark: dragon coiled around a döner skewer (1024×1024)
  reel.mp4        — 8s vertical 9:16 version of the brand film for Reels/TikTok
  story_teaser.jpg   — 9:16 "FEED THE DRAGON" teaser template (1152×2048)
  story_menu.jpg     — 9:16 menu card template with heat scale (1152×2048)
  story_history.jpg  — 9:16 "1972 INVENTED IT. WE SET IT ON FIRE." template (1152×2048)
```

## Design tokens

- Background `#0b0806`, panels `#14100c` / `#1a1410`
- Ink `#f5efe6`, muted `#a3978a`, hairline borders `rgba(245,239,230,.14)`
- Accents: ember red `#ff4a1c`, kimchi red `#d92e12`, torch yellow `#f5c542`
- Display font: condensed heavy all-caps (Anton or closest); body: Space Grotesk; labels: JetBrains Mono, wide tracking, uppercase
- All imagery carries the color; UI stays near-monochrome dark

## Sections (single long scroll, numbered editorial headers)

1. **Hero** — full-viewport looping `story.mp4` with dark bottom gradient, overlaid falling ember particle canvas (JS), giant "DRAGONDONER" display type (second word in ember red with glow), kicker "Berlin 1972 × Seoul Fire", subline about döner + kimchi uniting three food cultures, pill tags ("Kimchi-Infused", "Fine-Cut Vegetables", "3 Bread Traditions", "Exotic Sauces"), vertical scroll cue.
2. **The Story (01)** — manifesto grid: big condensed statement + body copy; side card "The Unique Hook: Döner was the first fusion. DragonDoner is the first fire."
3. **The Road to Fire (02)** — vertical history timeline: 1830s Bursa vertical spit → 1961–72 Gastarbeiter era → 1972 Kadir Nurman, Bahnhof Zoo, 1.50 DM (mention Aygün/Salim debate) → 1996 Gemüse döner revolution → 2026 DragonDoner kimchi fusion. Ember-red year numerals; final node glowing torch yellow.
4. **The Fusion (03)** — split panel: `ingredients.jpg` visual + copy on Anatolian flame / German craft / Korean fire; a 3-cell "trinity" strip (Türkiye — the spit & the flame; Germany — the bread & the crunch; Korea — the kimchi & the fire).
5. **Gallery** — drag-to-scroll horizontal strip of all five images plus the 9:16 `reel.mp4` as an autoplaying video frame; captions in mono; below it a "Social Kit" preview wall showing the three 9:16 story templates in phone-like frames.
6. **The Lineup (04)** — sticky `breads.jpg` beside a menu list: The Original Dragon €8.90, Kimchi Dürüm €8.50, Dragon Gemüse €7.90, Seoul Berlin Box €9.90, each with a ●-dot heat level and description; sauce rites pills: Dragon Sauce (gochujang×garlic yogurt), Torch Cream (smoked chili honey), Herb Riot (chimichurri fire).
7. **The Unification (05)** — `people.jpg` + copy about Berlin eating together regardless of nationality; stat strip: 3 food cultures · ~1,600 Berlin döner stands · 1 city.
8. **The Full-Stack Playbook (06)** — brand operating system in a grid: Brand Essence ("Migration is the mother of flavor. Fire is its language.") with Fire/Unity/Craft pillars; Audience (Berlin Purist, Korean diaspora & K-culture wave, Global street-food hunter, The night city); Voice & Copy ("Feed the dragon." / "mit scharf — dragon scharf." / "1972 invented it. We set it on fire."); Hook Machine (History/Fire/Unity/Heat hooks); Product System (three breads, fine-cut doctrine, sauce rites, Dragon Scale heat 1–5); Launch Sequence (90 days: Ignite the Legend → Feed the City → Spread the Fire).
9. **Partners in Fire (07)** — three cooperation cards linking out: DragonFest Berlin (dragonfestberlin.com), MangoFest Berlin (mangofestberlin.com), Instagram @dragondoner; cooperation line partners@dragondoner.com.
10. **Footer** — giant outlined "DragonDoner" wordmark (fills ember red on hover), dragondoner.com, credit line with both festival partners.

## Interactions

- Scroll-triggered fade/slide reveals (IntersectionObserver)
- Ember particle canvas floating over the hero video
- Pointer drag scrolling on the gallery strip
- Sticky menu visual; hover glow on outlined footer wordmark
- Fixed header with logo mark + nav (mix-blend difference), anchor links to all sections
- Fully responsive; video poster fallbacks; muted autoplay loops
