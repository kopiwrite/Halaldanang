# Claude — Working Memory (Halal Da Nang)

## Reading & deliverables SOP (HARD RULE)
- The user reads Markdown ONLY when pasted inline in chat as a ```markdown code block```.
- For ANY document/deliverable, GENERATE A PDF and send it inline (SendUserFile).
  Never tell the user to open a `.md`/file in the repo to read it.
- Short answers: inline chat. Anything structured/long: PDF inline.

## Image-handling guardrail (HARD RULE, from Trelinx local SOP)
- Never Read a PNG >= 3000px. Full stop.
- Precheck dimensions with Pillow before reading any image; if long edge > ~1800px,
  downscale a copy to <=1800px and Read that, never the original.
- HTML is the working surface; PNG is the human-review surface.
- User-pasted screenshots up to ~2500px = silent accept (don't flag).
- The guardrail targets images Claude pulls in, especially batches.

## Project facts
- Location: DA NANG (not Ho Chi Minh City). Grab storefront name: "Halal Online Home".
- Source of truth = the LIVE GrabFood store. See product-tree branch:
  PRODUCT_TREE.md / product_tree.csv. The old SOT.md is STALE — ignore it.
- Google Drive scope: "1. Duong Dang / Halal Da Nang" ONLY. Touch nothing else in Drive.
- Every write/edit needs the user's approval first.
- Binary -> Google Drive upload is NOT feasible from this cloud session (base64 must be
  hand-transcribed = unreliable). Deliver files INLINE instead. PDF/CSV(text) to Drive only
  if a Mac/local session does it (Drive-sync mount).

## Image generation
- Canva AI generator is weak at exact counts/plating. For art-directed food shots, the
  user runs Nano Banana (Gemini) with Claude-written prompts; results are good.
- Real product packet images: Open Food Facts URL -> Canva upload-from-url works.
