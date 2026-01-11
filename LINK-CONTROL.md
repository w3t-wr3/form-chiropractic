# Form Chiropractic - Link Control Guide

## Quick Toggle: Enable/Disable All Links

All homepage links are controlled by a simple CSS switch located in:
**File:** `css/clinic-hours.css` (lines 3-17)

---

## To DISABLE All Links (Current State)

Keep the CSS code **uncommented** (as it is now):

```css
/* ============================================
   LINK DISABLE SWITCH
   ============================================ */

a {
    pointer-events: none !important;
    cursor: default !important;
}

/* ============================================
   END LINK DISABLE SWITCH
   ============================================ */
```

**Result:** All `<a>` links on the homepage are non-clickable

---

## To ENABLE All Links

**Option 1 - Comment Out the Code:**
```css
/* ============================================
   LINK DISABLE SWITCH
   ============================================ */

/*
a {
    pointer-events: none !important;
    cursor: default !important;
}
*/

/* ============================================
   END LINK DISABLE SWITCH
   ============================================ */
```

**Option 2 - Delete the Code:**
Simply delete lines 10-13 entirely (the `a { ... }` block)

**Result:** All links become functional again

---

## Instructions for Claude

When you need to re-enable links, just tell Claude:

> "Open LINK-CONTROL.md and follow the instructions to enable all links"

Or simply say:

> "Enable all the links on the Form Chiropractic homepage"

Claude will know to comment out or remove the CSS block in `css/clinic-hours.css`.

---

## Technical Details

- **Method:** CSS `pointer-events: none` prevents all click events
- **Scope:** Affects ALL `<a>` tags site-wide (not just homepage)
- **Benefits:**
  - No HTML changes needed
  - Single line toggle
  - Preserves all link structure
  - Instant enable/disable
  - No JavaScript required

---

**Last Updated:** January 11, 2026
