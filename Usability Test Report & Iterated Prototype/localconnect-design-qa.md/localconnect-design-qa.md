# LocalConnect — Design and functional QA

Date: 10 November 2026. Selected visual: option 2, map-first discovery.

## Evidence

- Source visual truth: `../../outputs/localconnect/visual-concepts/concept-2.png` (852 × 1846 pixels).
- Implementation: `../../outputs/localconnect-screens/01-discover.png` (393 × 852 pixels).
- Browser viewport: 1400 × 1200 CSS pixels. Measured iPhone screen: 393 × 852 CSS pixels, scale 1. Pixel screen: 427 × 952 CSS pixels, scale 1. Screenshot density: 1 pixel per CSS pixel.
- Full comparisons: `comparison-before.png` and `comparison-after.png` in the screen evidence folder. Source downsampled to 393 × 852; implementation left at native capture size. Both images were opened together in each comparison.
- Focused comparison: `comparison-details.png`, source title/metadata/action/navigation versus implementation equivalents, opened together at readable size.
- Additional screen evidence: details, registration, confirmation, My events, list view, saved events, invalid form, cancellation, and Pixel discovery PNGs.
- State for source comparison: default discovery, Indiranagar, This weekend, selected gardening event, keyboard closed.

## Comparison history and fixes

1. **[P1] Main action covered by bottom navigation.** Initial discovery screenshot put the event action behind persistent tabs. Reduced top spacing and map height to fit the app-owned content within the smaller safe viewport created by required live device chrome. Post-fix capture shows the full View event button above tabs.
2. **[P2] Map pins lost semantic colours.** A generic button colour rule overrode pin colours. Added scoped pin colours. Post-fix capture shows cobalt, purple and orange pins with white symbols.
3. **[P2] List alternative had insufficient space.** Three event rows exceeded the short map region. List mode now expands the region to 280px. Browser verified all three rows and selected the third event successfully.
4. **[P2] Inactive flow content exposed to accessibility navigation.** Added app-owned active-screen gates without editing protected runtime files. Later details and registration AX snapshots contain only the current screen.
5. **[P1] Validation focus could scroll the outer device portal.** Changed programmatic field focus to `focus({preventScroll:true})`. Retested invalid submission on Pixel; device portal scroll position remained approximately zero (0.8px), with current screen intact. Clean Pixel discovery capture has correct status bar, content and navigation.

## Required fidelity surfaces

- **Typography:** DM Sans 400/600/700/800 approximates the geometric reference. Headline hierarchy and two-line wrapping match; event title, metadata and navigation remain readable. No substantive font wrapping issue in five-screen board.
- **Spacing/layout:** Location/search/map/event-sheet/navigation hierarchy preserved. Map is intentionally shorter than the source to accommodate the protected live status bar and home indicator while retaining the primary action above tabs. This is a device-safe-area adaptation, not an attempt at pixel-identical framing. Details scroll vertically and retain their fixed toolbar.
- **Colours/tokens:** White surface, near-black headings, muted metadata, cobalt actions and coloured pins match the selected direction. Focus/error states use distinct outlines/text. No full WCAG conformance claim is made.
- **Images/assets:** Generated map and gardening image visually match source subjects/crops; no raster screenshot is used as the app UI. Icons use Phosphor React. Optional second/third events use library icons rather than invented photos. Protected device, status and keyboard assets remain intact.
- **Copy/content:** Primary source copy retained. Added clear demo disclosures where booking/storage matters. Event names, venue, access and organiser data are explicitly fictional. No real booking, email or verified-organiser claim.

## Browser-tested interactions

Discovery → event detail → save → Saved retrieval; map/list toggle and selecting third result; empty query and reset; date filter sheet and All dates selection; registration required fields and invalid email recovery preserving the name; successful sample reservation; My events retrieval; cancellation confirmation and cancelled status; iPhone and Pixel discovery layouts.

Console error/warning check returned an empty list. Production TypeScript/Vite build passed. Mobile runtime integrity passed for all 28 protected files.

## Residual limits and polish

- [P3] Brand icon and generated photography are close visual equivalents, not identical source artwork. Source's decorative corner tint is omitted.
- [P3] The template's custom cursor appears in some interaction captures.
- Screen captures include required runtime chrome, which the source omitted. This expected difference is excluded from app-content fidelity findings.
- No participant usability study, formal assistive-technology audit, paid booking, live map, backend or durable storage. All three sample events fall within the same weekend, so All dates yields the same records.
- This is a coded prototype, not a Figma file. The assignment's Figma requirement remains outstanding.

## Implementation checklist

- [x] Correct action overlap, pin colours, list space, inactive content and focus scrolling.
- [x] Recapture and compare full discovery plus focused action region.
- [x] Verify main flow and meaningful recovery paths in Browser.
- [x] Preserve protected mobile runtime; build successfully.
- [ ] Create the required Figma prototype and conduct actual participant research/testing before claiming project completion.

final result: passed
