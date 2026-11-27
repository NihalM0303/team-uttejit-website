---
name: apple-design-system
description: Enforces the Team Uttejit Apple-style hardware-showcase design system (colors, type scale, spacing, glass nav, bento cards, motion) for every Framer page and component on the Team Uttejit website. Use whenever building or editing any page, section or component of the site.
---

# Team Uttejit — Apple-Style Hardware Showcase

Apply these rules strictly to every page, section and component. If a rule and a request conflict, follow the rule and say why.

## 1. Space and layout
- At least 40% negative space in every viewport.
- Max content width 1120–1200px, centred. Heroes, car imagery and video loops go full-bleed (100vw).
- Section padding: 96–144px top/bottom on desktop, 64px on mobile.
- Bento cards: radius 24px, 1px hairline border — `rgba(255,255,255,0.08)` on dark, `rgba(0,0,0,0.06)` on light. No drop shadows.
- Feature cards hold at most 2 short sentences. If copy is longer, cut it.

## 2. Surfaces and colour
| Token | Value | Use |
|---|---|---|
| `dark/canvas` | `#000000` | Home hero, Current Car page |
| `dark/card` | `#111113` | Cards on dark |
| `dark/text` | `#F5F5F7` | Primary text on dark |
| `light/canvas` | `#FFFFFF` | Editorial pages (About, History, Sponsorship, Leadership) |
| `light/card` | `#F5F5F7` | Cards on light |
| `light/text` | `#1D1D1F` | Primary text on light |
| `text/secondary` | `#86868B` | Captions, subheads, meta |
| `accent` | `#D90429` | ONLY primary CTAs, active nav state, key stats |

Never flood a background with the accent. No gradients, neon, or multi-colour badges.

## 3. Typography (Inter, fallback SF Pro / -apple-system)
| Style | Desktop | Mobile | Weight | Tracking | Line-height |
|---|---|---|---|---|---|
| Hero | 56–84px (default 80) | 36–44px (default 40) | 600–700 | -0.03em | 1.05 |
| Section headline | 40–56px (default 48) | 32px | 600 | -0.025em | 1.1 |
| Lead / subhead | 21–24px | 19px | 400–500 | -0.01em | 1.4 |
| Body | 17px | 17px | 400 | 0 | 1.55, max 65ch |
| Stat | 48–64px | 40px | 600, tabular-nums | -0.03em | 1 |
| Caption / eyebrow | 12–14px | 12px | 500–600 | 0.02em | 1.3 |

Hero headlines are 2–5 words. Never wrap a paragraph over an image.

## 4. Navigation
- Sticky 56px glass bar: background `rgba(0,0,0,0.72)` (dark) / `rgba(255,255,255,0.72)` (light), `backdrop-filter: blur(20px) saturate(180%)`, hairline bottom border.
- Logo left. Exactly 5 links: About, History, Current Car, Sponsorship, Leadership. One pill CTA "Partner With Us" (accent, radius 9999px) → /sponsorship.
- Active link uses the accent. Mobile collapses to a menu button.

## 5. Motion
- Reveal: opacity 0→1 + translateY 24px→0, ease `[0.22, 1, 0.36, 1]`, 0.6–0.8s, once.
- Image hover: scale(1.02) inside an overflow-hidden frame.
- Buttons: gentle opacity/brightness shift, no bounce.
- Respect `prefers-reduced-motion`.
- Videos: autoplay, muted, loop, playsInline, always with a poster image.

## 6. Content integrity
- Never invent specs, results, sponsors, people, or URLs. Facts come from `MEDIA_MANIFEST.md` and the sponsorship brochure.
- Missing media uses a labelled placeholder frame: `[16:9 — filename]`.
- Leadership details stay as placeholders until the team supplies them.

## 7. Copy tone
- Plain and factual. No hype words (revolutionary, challenger, unleash, backed by industry, etc.) and no slogans beyond the team's own tagline “Dream. Build. Revolutionize.”
- State what the team did, with dates and results. Short sentences. No exclamation marks.

## 8. Breakpoints
Check every page at 1440px (desktop), 834px (tablet) and 390px (mobile) before review.
