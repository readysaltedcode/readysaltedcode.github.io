# Content Refresh Strategy
## readysaltedcode - Recycling & Updating Legacy Content

---

## Executive Summary

The readysaltedcode website contains valuable educational content (6 lessons, 75 stories) created between 2012-2017. While the pedagogical approaches and creative concepts remain excellent, the technical references and presentation make the brand appear inactive. This strategy outlines how to refresh and recycle this content efficiently.

**Core Problem**: Content is 7-12 years old and references deprecated technologies, broken links, and historical events as if current.

**Solution**: A three-tier approach - Archive, Update, or Retire - applied systematically across all content.

---

## Content Inventory

### Lessons (6 total)

| Lesson | Status | Key Issues | Recommendation |
|--------|--------|------------|----------------|
| **Simple Wearables** | Evergreen | Minimal tech dependencies | Minor refresh |
| **Gemma** | Dated | Code from 2014, ATtiny85 | Update to modern Gemma M0 |
| **Piano Glove** | Dated | Flora being phased out | Update to Circuit Playground |
| **RC Car** | Moderate | AppShed still exists | Minor refresh |
| **Crumble** | Legacy | HTTP links, niche hardware | Archive or retire |
| **RPi-ano** | Outdated | ScratchGPIO deprecated, goo.gl link | Major rewrite needed |

### Stories (75 total)

| Category | Count | Examples | Approach |
|----------|-------|----------|----------|
| **Conference Reports** | ~25 | BETT2014, Scratch MIT 2016, BDF12 | Archive with dates |
| **Project Documentation** | ~20 | datadrivendance, wearables projects | Update as case studies |
| **Teaching Reflections** | ~15 | Curriculum thoughts, pedagogy | Review for relevance |
| **Announcements** | ~10 | "Coming soon", event promos | Retire or archive |
| **Technical Tutorials** | ~5 | Kinect, sensors | Update or retire |

---

## Three-Tier Content Strategy

### Tier 1: ARCHIVE (Historical Value)
Content that documents real achievements but shouldn't appear "current".

**Approach:**
- Add clear publication date header
- Add "Archive" or "Case Study" label
- Add context note: "This project was delivered in [year]. The technology has evolved but the approach remains relevant."
- Keep for credibility/portfolio purposes
- Move to dedicated "Archive" or "Past Projects" section

**Candidates:**
- Conference reports (BETT2014, Scratch MIT, etc.)
- Time-specific project documentation
- Event announcements that have passed
- Stories with heavy date references

**Template Header:**
```
Archive | Originally published [Month Year]
This case study documents work delivered in [year].
```

### Tier 2: UPDATE (Refresh & Recycle)
Content with strong pedagogical value that needs technical modernization.

**Approach:**
- Update technology references to current equivalents
- Fix broken links
- Refresh code examples
- Add "Last updated: [date]" notice
- Keep URL structure (preserve any existing SEO)

**Technology Update Map:**

| Old Reference | Modern Equivalent |
|---------------|-------------------|
| Kinect 360 | MediaPipe, Teachable Machine, webcam-based tracking |
| ScratchGPIO | Raspberry Pi Pico + MicroPython, or gpiozero |
| Adafruit Flora | Circuit Playground Express/Bluefruit |
| Adafruit Gemma | Gemma M0 or QT Py |
| Genuino 101 | Arduino Nano 33 BLE/IoT |
| AppShed | MIT App Inventor, Thunkable |
| Blockly (as novelty) | Blockly (standard tool) |
| goo.gl links | Direct URLs |

**Priority Updates:**

1. **RPi-ano Lesson** (High Priority)
   - Replace ScratchGPIO with Python + gpiozero
   - Remove goo.gl shortened URL
   - Update to work with Pi 4/5
   - Add micro:bit alternative

2. **Gemma Lesson** (Medium Priority)
   - Update to Gemma M0 (same form factor, better specs)
   - Update Arduino IDE references
   - Verify NeoPixel library compatibility
   - Update code examples

3. **Piano Glove Lesson** (Medium Priority)
   - Offer Circuit Playground Express alternative
   - Update sensor library references
   - Verify Adafruit Learn links still work

4. **datadrivendance Stories** (High Priority)
   - These are brand signature content
   - Update to case studies format
   - Add "currently available for booking" where applicable
   - Remove references to unavailable apps

### Tier 3: RETIRE (Remove or Redirect)
Content that's no longer useful or accurate.

**Approach:**
- Remove from main navigation
- Either delete or redirect to relevant updated content
- Document what was removed (for internal reference)

**Candidates:**
- "Coming soon" announcements that never materialized
- Extremely brief posts with no substance
- Password-protected content with no actual content
- Broken technical tutorials that can't be fixed
- Conference promos for events 10+ years past

---

## Implementation Plan

### Phase 1: Quick Wins (1-2 days)

**Technical fixes that don't require content rewriting:**

1. **Fix broken links**
   - [ ] Replace HTTP with HTTPS (Crumble lesson)
   - [ ] Replace goo.gl with direct URLs
   - [ ] Test all external links, note broken ones

2. **Add dates to all stories**
   - [ ] Add publication year to frontmatter
   - [ ] Display date on story pages
   - [ ] Add "Archive" label to pre-2020 content

3. **Fix broken embeds**
   - [ ] Update Flickr embed syntax
   - [ ] Update Twitter embed scripts
   - [ ] Remove or replace Flash objects

### Phase 2: Content Triage (1 week)

**Categorize all 75 stories:**

1. Review each story and assign to:
   - Archive (add date, keep as-is)
   - Update (flag for refresh)
   - Retire (remove or redirect)

2. Create new navigation structure:
   - "Resources" (current, updated content)
   - "Case Studies" (archived project documentation)
   - "Blog/News" (dated posts, clearly temporal)

### Phase 3: Priority Updates (2-4 weeks)

**Refresh high-value content:**

1. **Lessons** - Update the 4 viable lessons with modern tech
2. **datadrivendance** - Convert to evergreen case studies
3. **Signature Projects** - Google RISE work, key achievements

### Phase 4: Ongoing Maintenance

**Sustainable content strategy:**

1. Add "Last reviewed: [date]" to all lessons
2. Annual review cycle for technical accuracy
3. New content template with version/date fields
4. Consider removing very old stories entirely

---

## Story Refresh Approach

### For Conference/Event Stories
Transform from "I went to X" to "Key insights from X":

**Before:**
> "Just got back from BETT2014! It was amazing! Here are some photos..."

**After:**
> **Archive | BETT 2014**
> Key insights from our BETT 2014 exhibition, where we demonstrated wearable computing in education. This case study documents the approach we used to engage over 200 teachers...

### For Project Documentation
Transform from "we're working on X" to "how we delivered X":

**Before:**
> "We're excited to announce our datadrivendance project! Watch this space for updates..."

**After:**
> **Case Study: datadrivendance**
> datadrivendance combines classical ballet with real-time data visualization. Originally developed in 2015 with support from Arts Council England, the project has been performed at [venues] and adapted for school workshops.
>
> *This project is available for school residencies - [contact us](/workshops)*

### For Technical Tutorials
Either update fully or archive with warning:

**Option A (Update):**
> **Last updated: January 2026**
> This tutorial uses Gemma M0 and CircuitPython. For the original 2014 version using Gemma v1, see the archive.

**Option B (Archive with warning):**
> **Archive | 2014**
> *Note: This tutorial references Gemma v1 and Arduino IDE 1.x. The concepts remain valid but the specific code may need adjustment for current hardware.*

---

## Bulk Update Strategies

### Using Find & Replace
Some updates can be done programmatically:

```
# Technology references
"Kinect" → "motion tracking" (context-dependent)
"http://" → "https://" (where valid)
"goo.gl/Pthh62" → "[direct URL]"

# Date awareness
Add frontmatter: publishedYear: 20XX
```

### Stories Requiring Manual Review
- Any with "coming soon" or future promises
- Any referencing specific software versions
- Any with embedded media (check if working)

### Content That Can Be Bulk-Archived
- All conference reports pre-2020
- All stories with year in title (BDF12, BETT2014, etc.)

---

## New Content Structure

### Proposed Site Architecture

```
/resources
  /lessons          (updated, current tutorials)
  /lesson-packs     (purchasable content)

/case-studies
  /datadrivendance  (signature project)
  /projects         (past work, archived)

/workshops
  (current offerings)

/stories
  /archive          (dated blog posts, clearly labeled)

/about
  (credentials, awards, history)
```

### Adding Date Display

Update story template to show:
```astro
{story.data.publishedYear && (
  <span class="archive-badge">Archive | {story.data.publishedYear}</span>
)}
```

---

## Immediate Recommendations

### Do Now
1. Add publication years to all story frontmatter
2. Fix HTTP → HTTPS links in lessons
3. Replace goo.gl link in RPi-ano
4. Add "Archive" section to navigation

### Do This Month
1. Triage all 75 stories (Archive/Update/Retire)
2. Update RPi-ano lesson (highest technical debt)
3. Create "Case Studies" section for datadrivendance

### Do This Quarter
1. Update remaining lessons to current tech
2. Refresh top 10 most valuable stories
3. Remove/redirect retired content
4. Implement "Last updated" dates on all content

---

## Content Value Assessment

### Highest Value Content (Prioritize Updates)
1. **datadrivendance documentation** - Unique, brand signature
2. **Wearables lessons** (Gemma, Piano Glove, Simple Wearables) - Differentiated content
3. **Google RISE Award stories** - Credibility builders
4. **Workshop methodology posts** - Supports service sales

### Medium Value (Archive with Context)
1. Conference presentations/reports
2. Teaching reflections
3. Historical project timelines

### Low Value (Retire)
1. Brief announcements
2. "Coming soon" posts
3. Broken tutorials
4. Password-protected empty content

---

## Success Metrics

After refresh:
- [ ] No broken links
- [ ] All content dated (publication or "last updated")
- [ ] Clear distinction between current and archived content
- [ ] Lessons reference current (2024+) technology
- [ ] datadrivendance positioned as ongoing/bookable
- [ ] Stories support rather than undermine professional positioning

---

*Strategy document prepared January 2026*
*For discussion with Dr. Smith-Nunes*
