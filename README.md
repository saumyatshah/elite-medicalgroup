# Elite Medical Group

Website for Elite Medical Group — a primary care practice in Clarksville, Tennessee.

Family medicine, internal medicine, hospital medicine, and critical care with Dr. Parth Shah and Dr. Pankaj Shah.

## Practice

- **Address** 150 Alfredo Drive, Suite A, Clarksville, TN 37042
- **Phone** 931-271-7373
- **Email** elitemedgroupofclarksville@outlook.com
- **Hours** Monday – Friday, 8:00 am – 5:00 pm (closed for lunch 12–1 pm)

## Stack

Static site: `index.html` plus `assets/` (physician portraits) and `favicon.svg`. No build step. Fonts via Google Fonts (Fraunces + Newsreader). Appointment booking is an iframe/link to the practice's scheduling vendor (`d2oe0ra32qx05a.cloudfront.net`, `practiceKey=k_1_114082`).

## Relationship to the deployed site

`elite-medgroup.com` currently serves a compiled React/Vite bundle of this same design. This repo is the hand-maintained source of truth; its copy is **ahead** of what is live (see "Pending deployment" below).

## Local preview

```
python3 -m http.server 8787
open http://localhost:8787
```

## Pending deployment

Changes here that are not yet on `elite-medgroup.com`:

- Spelling corrected throughout: **Pankaj** (live still says "Pankhaj" in several places), full names "Dr. Parth Shah" / "Dr. Pankaj Shah" with an `MD` credential mark.
- Practice intro rewritten: locally owned / physician-led, serving Montgomery County, Christian County, and Fort Campbell.
- Practice heading "A team of board certified physicians" (live: "Two senior physicians").
- Physician tenure stated as *since 2009* / *since 2007*; credentials simplified to "Board-Certified, Family Medicine" / "Internal Medicine".
- Family medicine described as "from 12 and up"; Internal Medicine and Hospital Medicine descriptions shortened.
- Contact hours add the 12–1 pm lunch closure; the "After hours — Partner on-call" row and the "long memory" pull-quote are commented out.
- Email corrected to `elitemedgroupofclarksville@outlook.com`.
- Floating appointment-booking button (scheduling vendor iframe) in addition to the hero link.
