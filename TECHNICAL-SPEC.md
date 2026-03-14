# Aluma Broom — Technical Design Specification

## Version 1.0 — March 2026

---

## 1. CORE MECHANISM: "Razor-Slide" Attachment System

The Aluma Broom uses a **slot-and-bolt clamping system** inspired by how a razor blade seats into a disposable razor handle. The handle slides into a channel on the tool head, then two bolts coming **up from the bottom** are secured with **double wing nuts** on top.

### How It Works (Step by Step)

```
STEP 1: Slide the handle into the channel
================================================

        HANDLE (top view, cross-section)
        ┌──────────────────────────────┐
        │    Aluminum Flat Bar         │
        │    1.5" wide x 0.25" thick   │
        │  ○                        ○  │  ← Two bolt holes (slotted)
        └──────────────────────────────┘
                      │
                      │  slides into...
                      ▼
        ┌──────────────────────────────┐
        │  ┌────────────────────────┐  │
        │  │   CHANNEL / SLOT       │  │  ← Machined channel in tool head
        │  │   (razor-blade style)  │  │     1.55" wide x 0.30" deep
        │  └────────────────────────┘  │
        │         TOOL HEAD            │
        └──────────────────────────────┘


STEP 2: Bolts come up from the bottom
================================================

                WING NUT ──►  ╔╗    ╔╗  ◄── WING NUT
                              ║║    ║║
        ┌─────────────────────╨╨────╨╨─────────────────────┐
        │                HANDLE (in channel)                │
        ├─────────────────────╥╥────╥╥─────────────────────┤
        │                     ║║    ║║                      │
        │                TOOL HEAD BODY                     │
        │                     ║║    ║║                      │
        └─────────────────────╨╨────╨╨─────────────────────┘
                              ▲▲    ▲▲
                         CARRIAGE BOLTS
                    (come up from bottom,
                     square neck prevents spinning)
```

---

## 2. DETAILED CROSS-SECTION — Side View

```
                    WING NUT
                      ┌─┐
                     ╱   ╲
                   ╱       ╲
                  ├─────────┤
                  │  │   │  │
    ══════════════╪══╪═══╪══╪══════════════  ← HANDLE (aluminum flat bar)
                  │  │   │  │
    ──────────────┼──┼───┼──┼──────────────  ← CHANNEL WALLS (tool head)
                  │  │   │  │
                  │  │   │  │
                  │  │   │  │                ← TOOL HEAD BODY
                  │  │   │  │                   (broom frame / mop plate /
                  │  │   │  │                    squeegee bracket / etc.)
    ──────────────┼──┼───┼──┼──────────────
                  │  ▓   ▓  │                ← CARRIAGE BOLT square neck
                     ▓   ▓                      (sits in square recess,
                     ○   ○                       prevents bolt from spinning)

              BOLT HEADS (flush with bottom)
```

---

## 3. HANDLE SPECIFICATIONS

### Material: 6061-T6 Aluminum (Anodized)

| Spec | 18" Model | 24" Model |
|------|-----------|-----------|
| Overall length | 18 inches | 24 inches |
| Cross-section | 1.5" wide x 0.25" thick | 1.5" wide x 0.25" thick |
| Profile | Flat bar (rectangular) | Flat bar (rectangular) |
| Weight | ~0.45 lbs | ~0.60 lbs |
| Bolt holes | 2x slotted holes, 5" apart center-to-center | 2x slotted holes, 5" apart center-to-center |
| Hole size | 5/16" wide x 3/4" long (slotted for slide-in) | 5/16" wide x 3/4" long (slotted for slide-in) |
| Grip | Textured anodized finish or rubber overmold on upper 8" | Same |
| End cap | Rubber bumper cap (protects floors when leaning) | Same |
| Finish | Black anodized or brushed silver | Same |

### Why Flat Bar (Not Round Tube)?

The flat bar profile is critical to this design:
- **Slides into the channel** like a razor blade — impossible with a round tube
- **Anti-rotation** — the flat shape prevents the handle from twisting under load
- **Clamping surface** — wing nuts clamp flat-to-flat for maximum grip
- **Thinner storage profile** — flat bars stack/store more compactly than tubes

### Bolt Hole Detail

```
    ┌───────────────────────────────────────────────────────┐
    │                                                       │
    │   ┌───┐                                   ┌───┐      │
    │   │   │  ◄── Slotted hole                 │   │      │
    │   │   │      allows handle to              │   │      │
    │   │   │      slide in from the end         │   │      │
    │   └───┘      before bolts catch            └───┘      │
    │                                                       │
    │   ◄──────── 5" center-to-center ─────────►           │
    │                                                       │
    └───────────────────────────────────────────────────────┘
         ▲
         │ Slot opening faces the
           insertion end (open-ended)
```

The slots are **open on one end** (like a keyhole slot) so the handle slides in past the bolts, then you tighten the wing nuts. To remove: loosen wing nuts, slide handle out. 10-second swap.

---

## 4. TOOL HEAD DESIGNS

Each tool head has the **same standardized channel** on top for the handle, with the same bolt spacing. The only thing that changes is what's below the channel.

### 4A. Push Broom Head

```
         WING NUTS
          ╔╗  ╔╗
    ══════╬╬══╬╬══════  ← Handle (aluminum flat bar)
    ──────╬╬──╬╬──────  ← Channel receiver
          ║║  ║║
    ┌─────╨╨──╨╨─────┐
    │  BROOM FRAME   │  ← Injection-molded nylon or aluminum
    │   18" wide     │
    ├────────────────┤
    │▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓│  ← Stiff bristles (polypropylene)
    │▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓│     or soft bristles (flagged PET)
    │▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓│
    └────────────────┘

    Specs:
    - Frame: 18" wide x 3" deep x 1.5" tall
    - Bristle length: 3"
    - Total head weight: ~0.8 lbs
    - Options: Indoor (soft) / Outdoor (stiff) bristle sets
```

### 4B. Mop Head

```
          ╔╗  ╔╗
    ══════╬╬══╬╬══════  ← Handle
    ──────╬╬──╬╬──────  ← Channel receiver
          ║║  ║║
    ┌─────╨╨──╨╨─────┐
    │  MOP PLATE     │  ← Aluminum or ABS plate
    │  with Velcro   │     14" wide x 5" deep
    ├────────────────┤
    │░░░░░░░░░░░░░░░░│  ← Microfiber pad (Velcro-attached)
    │░░░░░░░░░░░░░░░░│     Machine washable, replaceable
    └────────────────┘

    Specs:
    - Plate: 14" wide x 5" deep
    - Pad attachment: Hook-and-loop (Velcro)
    - Included pads: 2x microfiber (wet/dry)
    - Head weight: ~0.5 lbs
```

### 4C. Squeegee Head

```
          ╔╗  ╔╗
    ══════╬╬══╬╬══════  ← Handle
    ──────╬╬──╬╬──────  ← Channel receiver
          ║║  ║║
    ┌─────╨╨──╨╨─────┐
    │ SQUEEGEE FRAME │  ← Aluminum channel
    │    18" wide    │
    ├────────────────┤
    │────────────────│  ← Dual-durometer rubber blade
    └────────────────┘     (firm core, soft edge)

    Specs:
    - Frame: 18" wide
    - Blade: Replaceable rubber, press-fit into channel
    - Head weight: ~0.4 lbs
    - Use: garage floors, shower glass, windows
```

### 4D. Duster Head

```
          ╔╗  ╔╗
    ══════╬╬══╬╬══════  ← Handle
    ──────╬╬──╬╬──────  ← Channel receiver
          ║║  ║║
    ┌─────╨╨──╨╨─────┐
    │  DUSTER PLATE  │  ← Slim ABS plate
    ├────────────────┤
    │ ≋≋≋≋≋≋≋≋≋≋≋≋≋≋ │  ← Electrostatic microfiber strips
    │ ≋≋≋≋≋≋≋≋≋≋≋≋≋≋ │     or chenille fingers
    └────────────────┘

    Specs:
    - Plate: 12" wide x 3" deep
    - Duster material: Washable microfiber chenille
    - Head weight: ~0.3 lbs
```

### 4E. Sander Head

```
          ╔╗  ╔╗
    ══════╬╬══╬╬══════  ← Handle
    ──────╬╬──╬╬──────  ← Channel receiver
          ║║  ║║
    ┌─────╨╨──╨╨─────┐
    │  SANDER PAD    │  ← Rigid foam-backed plate
    │  with Velcro   │     for sandpaper attachment
    ├────────────────┤
    │▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒│  ← Hook-and-loop surface
    └────────────────┘     (accepts standard sandpaper sheets)

    Specs:
    - Pad: 9" wide x 3.5" deep
    - Backing: Medium-density EVA foam (conforms to surface)
    - Attachment: Hook-and-loop for standard 1/3-sheet sandpaper
    - Head weight: ~0.35 lbs
    - Use: drywall, furniture refinishing, deck prep
```

### 4F. Shovel / Scraper Head

```
          ╔╗  ╔╗
    ══════╬╬══╬╬══════  ← Handle
    ──────╬╬──╬╬──────  ← Channel receiver
          ║║  ║║
    ┌─────╨╨──╨╨─────┐
    │  SHOVEL BLADE  │  ← Stamped steel or thick aluminum
    │   12" wide     │     with reinforced leading edge
    │                │
    │                │
    │                │
    └────────────────┘

    Specs:
    - Blade: 12" wide x 10" deep
    - Material: 14-gauge steel (powder-coated) or 3mm aluminum
    - Leading edge: beveled for scraping
    - Head weight: ~1.2 lbs
    - Use: snow, dirt, debris, ice scraping
```

---

## 5. THE CHANNEL RECEIVER — Universal Interface

This is the most critical component. Every tool head has this **exact same receiver** molded/machined into its top surface.

```
    TOP VIEW OF CHANNEL RECEIVER (on every tool head)
    ┌──────────────────────────────────────┐
    │                                      │
    │   ┌──────────────────────────────┐   │
    │   │        CHANNEL SLOT          │   │  1.55" wide x 0.30" deep
    │   │                              │   │  (handle is 1.50" x 0.25")
    │   │   ■                      ■   │   │  ← Square recesses for
    │   │   │                      │   │   │    carriage bolt necks
    │   │   ○                      ○   │   │  ← 5/16" bolt holes
    │   │                              │   │
    │   └──────────────────────────────┘   │
    │                                      │
    │           TOOL HEAD BODY             │
    │                                      │
    └──────────────────────────────────────┘

    ▲ OPEN END (handle slides in from this side)

    TOLERANCES:
    - Channel width: 1.55" (+0.00 / -0.02")  → snug fit on 1.50" handle
    - Channel depth: 0.30"                    → handle sits 0.05" below surface
    - Bolt holes: 5/16" diameter
    - Square recess: 5/16" x 5/16" x 3/16" deep (captures carriage bolt neck)
    - Bolt spacing: 5.0" center-to-center (matches handle slots)
```

### Hardware Per Tool Head

| Component | Spec | Qty |
|-----------|------|-----|
| Carriage bolt | 1/4"-20 x 1.25" long, stainless steel | 2 |
| Wing nut | 1/4"-20, stainless steel, stamped | 2 |
| Flat washer | 1/4" SAE, stainless steel | 2 |

**Bolts are permanently installed** in each tool head (square neck captures them so they don't spin or fall out). The user only handles the wing nuts.

---

## 6. STORAGE BOX

```
    ┌─────────────────────────────────────────┐
    │          ALUMA BROOM STORAGE BOX        │
    │              24" x 14" x 6"             │
    │                                         │
    │  ┌─────────────────────────────────┐    │
    │  │  HANDLE (18" or 24")            │    │  ← Foam-lined slot
    │  └─────────────────────────────────┘    │
    │                                         │
    │  ┌──────┐ ┌──────┐ ┌──────┐ ┌──────┐   │
    │  │BROOM │ │ MOP  │ │SQUEE-│ │DUSTER│   │  ← Individual
    │  │ HEAD │ │ HEAD │ │ GEE  │ │ HEAD │   │    compartments
    │  │      │ │      │ │ HEAD │ │      │   │
    │  └──────┘ └──────┘ └──────┘ └──────┘   │
    │                                         │
    │  ┌──────┐ ┌──────┐ ┌───────────────┐   │
    │  │SANDER│ │SHOVEL│ │  ACCESSORIES  │   │  ← Extra pads,
    │  │ HEAD │ │ HEAD │ │  sandpaper,   │   │    replacement
    │  │      │ │      │ │  mop pads     │   │    parts
    │  └──────┘ └──────┘ └───────────────┘   │
    │                                         │
    └─────────────────────────────────────────┘

    Material: Injection-molded ABS or corrugated polypropylene
    Lid: Snap-fit with carry handle
    Weight (empty): ~2 lbs
    Fits: under bed, in closet, garage shelf, RV storage bay
```

---

## 7. COMPLETE PRODUCT LINEUP

### Starter Kit — $79.99

| Item | Qty |
|------|-----|
| 18" Aluminum Handle | 1 |
| Push Broom Head (indoor) | 1 |
| Mop Head + 2 microfiber pads | 1 |
| Squeegee Head | 1 |
| Storage Box | 1 |
| Wing nuts + washers (pre-installed) | — |

### Pro Kit — $119.99

| Item | Qty |
|------|-----|
| 18" + 24" Aluminum Handles | 2 |
| Push Broom Head (indoor) | 1 |
| Push Broom Head (outdoor/stiff) | 1 |
| Mop Head + 2 microfiber pads | 1 |
| Squeegee Head | 1 |
| Duster Head | 1 |
| Sander Head + 3 sandpaper sheets | 1 |
| Storage Box | 1 |

### Ultimate Kit — $159.99

| Item | Qty |
|------|-----|
| Everything in Pro Kit | — |
| Shovel/Scraper Head | 1 |
| Extra microfiber pads (4-pack) | 1 |
| Extra sandpaper variety pack | 1 |
| Premium Storage Box (hard case) | 1 |

### Individual Heads (sold separately) — $14.99–$24.99 each

---

## 8. WHY THIS MECHANISM WINS

| Feature | Aluma Broom (Razor-Slide + Wing Nuts) | SWOPT (SnapLock Button) | Fiskars (QuikFit Clip) |
|---------|---------------------------------------|------------------------|------------------------|
| Lock strength | Bolt-clamped — will NOT come loose under load | Spring button — can pop off under heavy use | Plastic clip — wears over time |
| Tool-free? | Yes (wing nuts = hand-tightened) | Yes (push button) | Yes (squeeze clip) |
| Swap time | ~10 seconds | ~3 seconds | ~3 seconds |
| Failure mode | Graceful (wing nut loosens = wobble warning) | Sudden (button fails = head flies off) | Sudden (clip breaks = head falls) |
| Replacement parts | Standard hardware store bolts/nuts | Proprietary — must order from SWOPT | Proprietary — must order from Fiskars |
| Works when dirty/wet | Yes — metal threading doesn't care | Spring can jam with grit | Clip can stick with grit |
| Load capacity | Very high — clamped flat bar | Medium — single button detent | Medium — plastic clip |

**The trade-off is speed (10 sec vs 3 sec to swap), but the gain is reliability and strength.** For a product that includes a shovel and sander — tools that take real force — bolt clamping is the right call.

---

## 9. BILL OF MATERIALS (Per Starter Kit)

| Component | Material | Est. Unit Cost (at 5K units) |
|-----------|----------|------------------------------|
| 18" Handle | 6061-T6 aluminum, anodized | $3.50 |
| Push Broom Head | Injection-molded nylon + PP bristles | $4.00 |
| Mop Head | ABS plate + Velcro + 2 microfiber pads | $3.50 |
| Squeegee Head | Aluminum channel + rubber blade | $2.75 |
| Storage Box | Injection-molded ABS | $4.00 |
| Hardware (6x bolts, 6x wing nuts, 6x washers) | Stainless steel | $1.50 |
| Packaging + insert card | Cardboard + print | $1.50 |
| **Total COGS** | | **$20.75** |
| **Retail price** | | **$79.99** |
| **Gross margin** | | **~74%** |

---

## 10. NEXT STEPS

1. **CAD modeling** — Convert these specs into 3D CAD (SolidWorks or Fusion 360) for prototype printing
2. **3D print prototype** — Test the channel fit, bolt spacing, and wing nut ergonomics
3. **File provisional patent** — The "razor-slide channel + bottom-up carriage bolt + wing nut" combination is the patentable mechanism
4. **User testing** — Have 5-10 people swap heads and give feedback on the wing nut tightening experience
5. **Kickstarter prep** — Prototype video showing the slide-in, clamp-down, swap-out workflow
