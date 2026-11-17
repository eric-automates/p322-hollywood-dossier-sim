# SIMULATED ORDNANCE DOSSIER — Hollywood-Style 1980s Report Pastiche & WebGL .22 LR Ballistics Toy

> **FICTION · SIMULATED EDUCATIONAL AND FORMATIVE USE ONLY · NOT A REAL DOCUMENT**

---

## ⚠️ DISCLAIMER — READ FIRST

**THIS REPOSITORY IS A SIMULATION PROVIDED FOR EDUCATIONAL AND FORMATIVE PURPOSES ONLY.** The word *formative* is used deliberately: this is a visual-literacy, document-design, and browser-physics exercise — a learning artifact to be looked at and studied as a piece of crafted fiction. It is a depiction to be examined, not a reference to be consulted, and it must not be read, cited, or relied upon as a source of facts, guidance, or direction for any real-world purpose.

**IT IS MEANT TO LOOK LIKE A HOLLYWOOD DEPICTION OF A REPORT, NOT LIKE A REAL REPORT.** The 1980s government/military ordnance-dossier styling — aged bond paper, stencil and typewriter typography, invented `TM`-style document numbers, department headings, rubber stamps, "declassified" redaction bars, figure/table/paragraph numbering, and bureaucratic prose — is a **deliberately theatrical, dramatized movie-prop aesthetic**. It is a pastiche, a costume, a stage set. It is **not** a scan, reproduction, facsimile, reconstruction, or imitation of any genuine archival record.

**NOTHING IS MEANT TO LOOK REAL, BE REAL, OR BE MISTAKEN FOR SOMETHING REAL.** No document, form number, stamp, seal, marking, log entry, telemetry readout, or "official" heading shown here is authentic. Any resemblance to any actual publication, agency form, technical manual, record, or person is coincidental and purely stylistic. Nothing in this repository should be treated, referenced, shared, or presented as a genuine government, military, law-enforcement, or manufacturer document.

**NO AFFILIATION, SPONSORSHIP, APPROVAL, OR ENDORSEMENT.** This project is not authored, issued, approved, endorsed, sponsored by, or affiliated with the U.S. Government, the U.S. Department of Defense, the U.S. Army, the Bureau of Alcohol, Tobacco, Firearms and Explosives, the U.S. Department of Justice, SIG Sauer, Inc., or any government agency, military body, law-enforcement organization, standards body, or firearms manufacturer. Product names and trademarks appear solely as nominative references to identify the subject of the simulation; all trademarks remain the property of their respective owners, and no endorsement is implied.

**NOT A MANUAL, NOT TRAINING, NOT ADVICE, NOT A GUIDE.** Nothing here constitutes an operator's manual, armorer's guide, gunsmithing guide, safety guide, legal advice, legal opinion, or procurement, sourcing, modification, handling, or usage instruction of any kind. Do not rely on this repository, or on anything rendered by it, for any decision or action outside of a browser.

**EVERYTHING ON SCREEN IS SIMULATED.** The 3D model, mechanical interlocks, acoustics, chronograph values, trajectories, dispersion, target impacts, carrier motion, telemetry, and "ordnance log" text are software approximations generated for visualization inside a fictional framing device. They are not measured, tested, certified, validated, or authoritative, and no warranty is made as to their accuracy. The downrange 3D lane is compressed and display-scaled; the site says so on screen.

**NO CONDONING OR ENABLING OF UNLAWFUL CONDUCT.** The simulated "SIM-AUTO [TEST ONLY]" toggle is a clearly labelled software timing loop and a red label only — no conversion-device hardware is depicted, modelled, described mechanically, or made available. The statutory references included in the simulated dossier are limited public-record vocabulary and civic-law context placed inside a work of fiction; they contain no mechanical descriptions, dimensions, diagrams, files, print settings, part numbers, sourcing, acquisition, assembly, fitting, or installation details, and they are not legal advice. Unlawful possession or manufacture of a real machinegun conversion device is a federal felony; this project does not condone, encourage, facilitate, recommend, or enable it.

**NO WARRANTY / NO LIABILITY.** Provided "AS IS," without warranty of any kind, express or implied. The author(s) and contributor(s) accept no liability for any use, misuse, interpretation, or reliance. If you are publishing a fork, keep this disclaimer intact and visible.

---

## What this is

A single, standalone `index.html` — zero dependencies, zero CDNs, zero network assets — that runs entirely offline and is ready for GitHub Pages. It is a piece of interactive fiction dressed as a 1980s ordnance report, built around:

- A 360°-orbitable, directly manipulable WebGL 3D pistol model whose slide, magazine, trigger, safety, slide catch, takedown lever, and muzzle device respond to dragging and clicking — with hollow CNC slide/barrel/muzzle through-bores in Field-Strip (`STRP`) mode, exact `0–20` (`20+1`) and `0–25` (`25+1`) X-Ray cartridge stacks, an orange anti-tilt follower, and a dynamically compressing zig-zag magazine spring.
- Multi-chamber compressible propellant gas, internal flame, and recoil simulation: upward and 45°-angled compensator port flame jets, muzzle-device recoil/flip mitigation across both ported compensators and suppressors, cumulative multi-baffle swirling gas vortices that build across rapid or simulated cyclic bursts and slowly bleed down between strings (resuming from live residual pressure on follow-up shots), and 3D-projected X-Ray sensor pins with angled leader-line PSI readouts across the chamber, upper breech, barrel bore, magazine well, and muzzle/canister.
- A **true 4-border perimeter instrument bezel** (plus a top-strip `OPEN LIVE CONSOLE` ↔ `✕ CLOSE LIVE CONSOLE` toggle): every actuator sits shoulder-to-shoulder around the four outer edges of the 3D viewport as compact square and round SVG-icon pads with short stencil codes, keeping all four borders (top, left, right, and bottom) and the 3D pistol/target on the **same screen simultaneously** on both phone portrait and desktop — no hidden edge tabs and no controls stacked below the fold. The top border holds cartridge selection, camera/view/mode dials, glossary/telemetry/fullscreen toggles, and simulated cyclic-test controls; the left border holds mechanical actuators; the right border holds muzzle devices, four iron-sight sets plus the direct-mount **SIG ROMEOZero 3 MOA Red Dot (`RDOT`)**, and buyable-part toggles; the bottom border holds the target carrier (`DPLY`, `T1/5`–`T5/5` target-type cycle, `7YD–100Y` yardage, `INSP` close-up target inspection, `FRSH`, `SHOT`), holdover/windage dials, and guided demos.
- A **clickable 47-term illustrated glossary** (`GLOSSARY` top button + `Appendix G` index + dotted-underlined words throughout the text): clicking any highlighted technical term opens a pop-up card with a custom schematic SVG visual aid, plain-language explanation, clickable related-term pills, and jump links to deeper sections.
- A Web Audio acoustic model across six `.22 LR` cartridge profiles and four muzzle configurations.
- A downrange 3D target carrier on an overhead rail: **five swappable target faces** (NRA B-8 bullseye, AR500 steel gong, B-27 silhouette, 1-inch MOA sight-in grid, and an LE **Hostage Rescue Qualification** target with Threat Cranial T-Box / Thoracic A-Zone vs. foreground No-Shoot Hostage penalty scoring), six yard lines from 7 to 100 yards, pull-in inspection that toggles to "send target back out," punched bullet holes, a swinging AR500 gong with a flight-time-delayed impact sound, and live exterior-ballistics readouts.
- A first-person sight-picture aiming view supporting four iron-sight sets and a panoramic hooded **SIG ROMEOZero 3 MOA red-dot reflex window**, complete with holdover, windage, breathing sway, and Gaussian group dispersion.
- A fictional "Custom Shop" of real, commercially available accessory categories with swappable 3D iron sights, direct-mount micro red-dot reflex optic, 25-round extended magazine, ported compensator, skeletonized flat trigger, and M1913 rail light.
- Eight staged, progressively detailed sections written in the invented bureaucratic voice of the fake report.

It's a **toy for looking at**, in the same way a prop master's binder or a movie's fictional dossier is a toy for looking at — plus some genuinely fun browser physics.

## What this is not

| Not this | Because |
| --- | --- |
| A real technical manual or archival document | Every number, stamp, seal, and heading is invented stage dressing. |
| An official or affiliated publication | No agency, military body, or manufacturer authored, approved, or endorsed it. |
| Firearms instruction, training, or gunsmithing guidance | It is a simulation with no procedural content for real equipment. |
| Legal advice | Statutory mentions are fictional framing context, not counsel. |
| A source of measured or certified data | All values are software approximations for visualization. |
| A depiction or model of any conversion device | None exists anywhere in the project. |

## Repository description (paste into GitHub → About → Description)

```
SIMULATED EDUCATIONAL & FORMATIVE USE ONLY. A Hollywood-style fictional 1980s 'ordnance report' pastiche + offline WebGL SIG P322 ballistics sim. Nothing is meant to look real or be taken as authentic. No affiliation/endorsement; no instructions or advice.
```

*256 characters — within GitHub's 350-character limit, with the disclaimer leading so it is visible even where descriptions are truncated.*

Suggested topics: `simulation` · `fiction` · `hollywood-prop` · `webgl` · `educational` · `standalone-html` · `github-pages` · `ballistics-sim`

## Run it

No build step, no package manager, no install.

```bash
# Option A — just open the file
open index.html          # macOS
xdg-open index.html      # Linux
start index.html         # Windows
```

```bash
# Option B — serve locally (optional; file:// works too)
python3 -m http.server 8000
# then visit http://localhost:8000
```

### Publish on GitHub Pages

1. Create a repository (suggested name: `p322-hollywood-dossier-sim`).
2. Add `index.html` and this `README.md` at the repository root.
3. **Settings → Pages → Deploy from a branch → `main` / `root`.**
4. Paste the repository description above into **About → Description**.
5. Add a `LICENSE` file of your choosing before publishing.

Everything is inline (CSS, JavaScript, WebGL shaders, Canvas2D target textures, Web Audio synthesis). There are no external fonts, scripts, images, or API calls, so the site also works fully offline and inside restricted networks.

## Simulation notes

- The exterior-ballistics model is a closed-form exponential-drag approximation calibrated against published `.22 LR` pistol chronograph figures — not a six-degree-of-freedom solver. Real ammunition lots, barrels, temperatures, and elevations vary.
- Downrange 3D distances are compressed to keep a 100-yard target inside a browser viewport; the on-screen HUD repeats this notice. Numeric drop, time of flight, wind drift, and dispersion are computed at true yardage.
- The sight-picture view uses a simulated magnified laboratory optic so holdover is legible; impact coordinates remain computed in real inches.
- Group sizes, sound pressure values, and mechanical behavior are illustrative approximations, not guarantees or measurements.

## Legal, safety, and attribution

Repeating the controlling point: **this is a simulated, fictional, Hollywood-styled educational and formative artifact. Nothing is meant to look real, be real, or be taken as real.** It is not affiliated with or endorsed by any government agency, military organization, law-enforcement body, or manufacturer. It contains no instructions, no advice, and no actionable content of any kind, and it does not condone or enable unlawful conduct. Trademarks are used nominally and remain the property of their owners. Provided "AS IS," with no warranty and no liability.

If you fork, mirror, screenshot, or embed this project, keep the disclaimer attached and visible — especially in screenshots, where a cropped fake "TM" page could otherwise be detached from its context.

---

*Fictional document design · browser-native WebGL1 + Web Audio · single-file HTML · no external assets · no network calls.*
