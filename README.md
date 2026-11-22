# RootFrond — Landing Page

A project-aligned update of the **original cocoNet landing-page codebase**. The layout, CSS styling, interactive components, image assets, section IDs, and marked team-member code blocks have been retained. Only project content and a few small compatibility/accuracy fixes were changed.

## Project purpose

RootFrond is a proposed soil-and-leaf nutrient assessment system for Sri Lankan coconut growers. The concept uses portable **NPK sensors** for estimates of nitrogen (N), phosphorus (P), and potassium (K), plus pH, electrical conductivity (EC), moisture and temperature measurements. **Coconut leaf/tree image analysis** is intended to cross-check the sensor estimates. Once validated, combined information could help farmers understand nutrient status and consider fertilizer options and estimated costs in LKR.

These are **planned capabilities**, not a functioning product. Sensor calibration, laboratory comparison, AI model training, and field validation are still necessary.

## Run locally

1. Extract the ZIP.
2. Open `index.html` in a browser, or use VS Code Live Server.
3. Keep `style.css`, `script.js`, and the `images/` folder in the same relative locations.

No build step is required. Google Fonts and Lucide icons use external CDNs; their fallbacks may display differently when offline.

## Directory structure

```text
RootFrond_Exact_Site/
├── index.html
├── style.css
├── script.js
├── images/
│   ├── rootfrond-overview-bg.png  # Your supplied coconut-grove image
│   ├── rootfrond-favicon.svg      # Simple RootFrond tab icon
│   └── (original team portraits and site images)
├── README.md
└── TEAM-GUIDE.md
```

## Team ownership preserved

| Member | Existing assigned sections | Where to edit |
|---|---|---|
| Anupama | Overview + FAQ | Anupama HTML/CSS/JS comment blocks |
| Janith | How It Works | Janith HTML/CSS/JS comment blocks |
| Janani | Nutrient Analysis | Original `disease-detection` HTML ID and Janani code blocks |
| Sudil | Farmer Insights | Original `farmer-stories` HTML ID and Sudil code blocks |
| Isindu | Team + Get Involved + app preview | Isindu HTML/CSS/JS comment blocks |

The IDs `#disease-detection` and `#farmer-stories` are **intentionally unchanged**, to avoid breaking existing CSS/JS and internal links, even though the displayed headings now describe RootFrond.

## Background image

The provided coconut-grove image is included at `images/rootfrond-overview-bg.png` and is applied only to the existing Overview hero with a soft overlay in light and dark modes. You can swap the file without editing HTML or JavaScript.

## Pre-publication checklist

- The mobile-app views are **illustrations**, not connected to a sensor or AI model.
- The six Farmer Insights cards are **hypothetical scenarios**, not actual farmer testimonials or ratings.
- The form **downloads a text file** with the visitor's entries. It does not send an email, store data, or join a waitlist. Connect an approved form endpoint or mailbox before advertising registration.
- Replace the original frond-disease image used as illustrative artwork with a more appropriate image if the team has one and permission to use it.
- Confirm team members' names, titles and roles against the team's official records: the original website and original README do not use exactly the same name for one member.
- Do not claim quantitative nutrient accuracy, instant fertilizer recommendations or app-store availability until implementation and validation support them.

## Academic context

Developed for the Agile Team Project at IIT, affiliated with the University of Westminster. Keep the team's Git history in its existing repository; the packaged release omits `.git/` metadata.
