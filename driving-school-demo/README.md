# Apex Driving School — Demo Site

A single-page static demo built to show prospective driving instructor
clients what PhoenixFlow can build for them. No backend, no build step —
just `index.html`.

## Placeholders to swap for a real client

- **Business name / logo**: "Apex Driving School" — appears in nav, hero badge, footer, and `<title>`/meta tags.
- **Tagline & copy**: hero headline, sub-copy, stats (`96%`, `12 yrs`, `500+`) are illustrative — mark stats as unverified or replace with the real instructor's numbers.
- **Pricing & durations**: Standard Lesson, Intensive Course, Motorway Lessons, Test Prep — all placeholder prices.
- **Instructor bio**: name "James Doyle", initials avatar, experience, and badges are placeholders — swap the avatar `<div class="instructor-photo">JD</div>` for a real `<img>` once you have a photo.
- **Testimonials**: three placeholder reviews — replace with real client quotes (with permission).
- **Contact details**: phone (`+44 1234 567890`), email (`hello@apexdrivingschool.co.uk`), WhatsApp (`wa.me/441234567890`) are all placeholders.
- **Booking links**: every "Book" button points to `https://cal.com/apex-driving-demo` (and sub-paths like `/standard-lesson`, `/intensive-course`, `/motorway-lesson`, `/test-prep`). Once the real Cal.com username and event types are set up, do a find-and-replace of `apex-driving-demo` → the real Cal.com username, and update the event slugs to match.

## Deploying to Netlify

**Option A — drag and drop (fastest for a demo):**
1. Go to https://app.netlify.com/drop
2. Drag the `driving-school-demo` folder onto the page.
3. Netlify gives you a live URL immediately.

**Option B — connect this repo:**
1. In Netlify: *Add new site → Import an existing project*.
2. Point it at this repository.
3. Set **Base directory** to `driving-school-demo` and **Publish directory** to `.` (already configured in `netlify.toml`).
4. Deploy — no build command needed, it's static HTML.

**Option C — Netlify CLI:**
```bash
npx netlify-cli deploy --dir=driving-school-demo --prod
```
