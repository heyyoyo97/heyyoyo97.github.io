# Hand-ink cats v2

Created with built-in image_gen, 2026-09-14. Selected style: A, with corrected outward cheek whiskers. Raw raster sheets are preserved; CatArt uses SVG viewports and luminance masks to render the ink in semantic colours. No raster paper or white body fill is displayed. Thread sprites use the separate silhouette matte as a page-coloured backing, so the yarn is hidden only behind their bodies. The corrected ink sheet contains a generated checkerboard; the luminance transfer excludes that entire light range, while the silhouette matte controls occlusion. No checkerboard is rendered.

Character sheet origin: built-in image_gen output exec-225e72f7-c632-4e33-a288-64768dad550d.png, approved three-pose study in this conversation.

## hero.png

Generate production illustration asset: TWO animation keyframes of SAME relaxed person with SAME cat lying together, vertically stacked with enormous clear separation. Reference1 is approved HERO relationship and clothing, reference2 is approved cat line style. Remove ALL text, headline and UI. Landscape 1536x1024 white pure #ffffff background. Top scene entirely inside x100..1436 y70..440; bottom same scene entirely inside x100..1436 y590..960. Equal scale same body footprint aligned precisely. Person lies horizontally, feet LEFT head RIGHT, head very small, simple dot features with dark hair and loose shirt/pants; make posture MORE RELAXED than reference: one knee softly bent higher, other leg extended loosely at slight angle, rounded relaxed shoulders, one arm behind head, other forearm resting by cat. Torso not a long stiff rectangle, clothing loose, limbs coherent. Cat lounges on person's torso, same original angular uneven ears dot eyes thick felt pen wry cat. TWO short whiskers OUTWARD on each CHEEK, no forehead marks. TOP resting state: cat resting chin near person's shoulder, person looking toward cat. BOTTOM interaction state: human body stays exactly same, cat lifts small head and extends one forepaw toward person's hand/cheek, face still visible. Do not change full scene footprint between frames. Same dark #20221d imperfect medium-heavy felt pen, no sketch hatching, no polished vector aesthetic, no exaggerated cute eyes. Body interior pure white same as background; hair dark. NO shadows, gray background, gradients, texture, ground line, decorations, accessories, lettering, signature. Complete uncropped scenes, production illustration sheet not screenshot.

## thread.png

Production cat animation sprite sheet. Use attached approved character study as STRICT style and character reference: original awkward economical felt pen cat, uneven pointed ears, dot eyes, tiny nose, TWO SHORT whiskers pointing OUTWARD from each cheek, never forehead, heavy naturally imperfect dark ink line. Create precisely NINE separate full-body drawings in evenly spaced 3 by 3 grid on pure WHITE. All face RIGHT, equal cat BODY size, paws on same baseline per row. NO balls or toys in any cell, code draws ball separately. Each cell generous margin, ears/tails fully contained, NO overlap between cells. Row1: seated cat REST with front paws down; same seated cat BAT with right forepaw extended right toward imaginary ball; CHASE cat leaning forward in short crouching step. Row2: low stalking cat REST crouched with face lifted; same low cat BAT reaching forepaw a little farther; CHASE low cat stretched forward crawling. Row3: cat reclining on its SIDE REST head up facing right; same cat on side BAT both forepaws reaching to right to catch imaginary ball; CHASE cat rolling slightly onto back, head at right and forepaws extended toward right. Group silhouette remains consistent within each row; clear whole-pose changes between rows. White body same as background, black #20221d ink only, NO words numbers labels gridlines shadows groundlines paper noise shading fur hatching. Do not become detailed or cute rounded vector mascot. Production 1536 square illustration sheet, clean white blank corridors between cells.

### Thread alpha extraction

Edit this exact production 3x3 cat sprite sheet. Background extraction ONLY. Preserve EVERY cat's pixels, pose, size and position exactly, preserve square canvas dimensions and all nine cells. Remove ONLY the exterior white paper background to genuine transparent alpha, including exterior empty spaces between legs and tails. KEEP enclosed white BODY INTERIORS fully opaque white, so each cat is a solid opaque cutout with black ink outline and white body. Preserve anti-aliased contour edges. Absolutely no redraw, no movement, no new details, no missing cats, no background halo or checkerboard painted into the image. Result PNG true transparent background and opaque white-bodied cats. Image layout unchanged, this is a sprite alpha extraction.

## circle.png

Production decorative illustration for a portfolio. Exactly THREE small cats arranged head-to-tail around an EMPTY circular center, each cat follows the circle tangentially in a different orientation as if chasing each other clockwise. NO drawn circular line. Use attached cat style reference for same economical awkward original feline: irregular thick felt-pen ink, angular mismatched ears, tiny dot eyes, short notched legs, two SHORT outward whiskers per cheek, no forehead whiskers. All three cats same body size and style, relaxed fluid slightly crooked shapes, clear spacing between tails and next heads, NOT connected. Circular arrangement centered with generous outer margins. Pure white background and white cat interiors, dark #20221d ink only, no shadows gradients gray wash grain hatching labels text signature or watermark. Square canvas. This will rotate gently as a complete group on webpage, so make circular composition balanced and complete uncropped tails. Original drawings not copied from reference, reference used for character consistency.

## pair.png

Production TWO-FRAME illustration sheet of a humorous double-cat cheek tap. Attached original cat reference sets drawing language: angular slightly unequal ears, tiny dot eyes, short legs, thick naturally imperfect felt pen, economical lopsided shapes, deadpan mood. Landscape sheet TWO panels side-by-side on solid pure white, no panel borders. In EACH panel exactly TWO small sitting cats: left cat seen mostly from back/three-quarter, right cat faces viewer. Left panel REST: left cat forepaw slightly lifted near right cat's cheek, right cat sitting calmly, tiny dot features. Right panel TAP: left cat extends ONE paw touching right cat's cheek gently, right cat tilts head a little away. Gentle comic gesture not fighting. Same pair body scale, position and footprint between both frames. Two short whiskers outward from each visible cheek, no lines on forehead. White interior matching pure white background, dark #20221d ink only, no shading no shadows no fur texture no words no signature no watermark. Broad empty gaps between the two pairs, each pair centered in its half, complete uncropped bodies and tails. Clear compact horizontal composition suitable for display as a very small webpage illustration. Preserve original character not detailed realistic anatomy or polished vector mascot.


## Final side-head correction

The user rejected diagonal frontal heads on side-facing poses, particularly
row 2. `thread.png` is the corrected three-quarter head sheet. The intermediate
cutout was superseded; its generation history is retained in `prompts.json`.
`thread-silhouette.png` follows the corrected silhouette and supplies body
occlusion independently of the ink. All six source rasters embed their exact
prompt or prompt chain under the `impeccable:prompt` PNG metadata key.

`prompts.json` is the final per-file prompt set. Built-in image_gen was used for
all production assets; no CLI model or third-party character assets were used.

## Shelf peek and Hero gesture refinement

`shelf.png` (1254 square) is a built-in image_gen parts sheet: the head and
two paws are cropped independently; code adds pupils inside the empty eyes.
The head rises while the paws stay on the shelf baseline. Pupils follow the
selected book, and keyboard exit resets the scene.

`hero-cover.png` (1536 by 1024) is a built-in edit of `hero.png`, strengthening
the lower-frame gesture: the cat reaches to the person's forehead and the
person closes their eye. The original resting image remains in use.
Exact generation prompts are recorded in `prompts.json`.

The shelf sheet was subsequently redrawn using `hero.png` as the direct
character reference: short unequal ears, no inner-ear or cheek-fur details,
two blunt whiskers per cheek, small eyes and simple paws. The shelf mask adds
seven source pixels of ink dilation so the contour retains its weight at
110px display width. Pupils and gaze range are calibrated to the smaller eyes.

`thread-pounce.png` replaces the middle group's active pose with a low crouch
and both forepaws planted forward. It is used only for group 1's `bat` state,
so the first and second stages no longer share the same single-arm gesture.

## Not-found page

`not-found.png` is a 1774 by 887 two-frame sprite generated with built-in
image_gen. It shows one seated cat wearing an orange traffic cone: the resting
frame keeps the cone upright, while the interaction frame tilts it. CSS selects
each half for pointer, keyboard and touch activation; reduced motion keeps the
resting frame. The exact prompt is recorded in `prompts.json`.
