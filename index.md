
# A technique for accurate laser cutting on upside-down digital prints. A tutorial on how to make zero-kerf laser-cut jigsaw puzzles.

This method uses a Measurement and Alignment (MAP) sled, the goal being "naked-eye perfect" cut alignment.

<p class="error"><b>This is not a beginner-level technique.</b> If you've never made a laser-cut jigsaw puzzle before, start with one of the many simple tutorials easily found on YouTube.</p>

<p class="error">
<b>Fair warning for experienced puzzle makers:</b> this is a laborious way to make a puzzle. (Also expensive, for larger puzzles.)  Continue only if you have a serious peeve against loosely-fitting puzzles, or you have some other use for the precision upside-down cutting technique.</p>

<p class="info">Any comments or questions may be posted <a href="https://community.glowforge.com/t/kerf-adjusted-jigsaw-puzzles-tutorial/121437">in the Glowforge forum.</a></p>


## 90-second video overview

This quick video shows the essence of the precision cutting technique, and also serves as the companion video for Part 1 of the tutorial.

{% include youtube.html id="bI3UKxNdW8M" %}

## Tutorial

- [Part 1: Using the Alignment Sled](using-the-alignment-sled.md) — Detailed walk-through with prepared example files
- [Part 2: Single-page puzzles](single-page-puzzles.md) — How to create your own vector files
- **Part 3: [forthcoming] Masking and de-masking (weeding)** — Discussion; weeding trick
- **Part 4: [forthcoming] Multiple-page puzzles** — How to create your own vector files; how to mitigate relative error

## Supplementary

* [Jigsaw template generator for 2D pieces instead of 1D edges](https://mchrisman.github.io/jigsawGenerator/)
* [Example of micro puzzles created using this technique](https://community.glowforge.com/t/christmas-russian-doll-jigsaw-puzzles-micro-puzzles/121318)

## Q & A

#### Is "naked-eye perfect" alignment even possible?
The short answer: Just barely ... usually ... depending on the use case.

* Jigsaw puzzle pieces should be relatively aligned within 0.2mm (depending on photo, resolution, piece size).
* Small puzzles cut from a single page appear perfect, because errors in adjacent pieces tend to cancel out.
* My own Glowforge is only accurate to 0.1mm (after compensating for scale and drift)
* I can usually place cuts with error under 0.2mm.

I'll share the long answer later.

#### Why cut upside-down?
Because in laser cutting, the kerf is always wider on top, narrower on the bottom.  For jigsaw puzzles, if you want the kerf reduced or eliminated on the front face, you need to cut it upside-down.

#### What is this good for?
* Making zero-kerf puzzles
* Accurately cutting out shapes from a picture
* Seamlessly joining halves of an oversized puzzle
* Cutting individual pieces (e.g. replacements)
* Scoring the back sides of prints, for origami fold lines.

#### What is the MAP sled solving (that can't be solved with a ruler and stationary jig)?

It compensates for:

1. Glowforge's coordinate system origin can shift every time it recalibrates itself (millimeter-scale errors can happen)
2. Glowforge's coordinate system origin can drift over time (sub-millimeter-scale errors are typical)
3. Glowforge's coordinate system can be slightly out of scale (relative to the "real-world" distances defined by your favorite ruler).
4. The **position** and **size** of the printed image on the page isn't predictable. (Large-scale errors are seen due to bleed or idiosyncracies of the printer. From page to page, unpredictable millimeter-scale differences of position and sub-millimeter-scale differences of size are typical.)

The sled is designed to directly align the printed image's boundaries with Glowforge's coordinate system, without the intermediate step of going through the (irrelevant) real-world coordinate system.  The sled is disposable and generally single-use because of (1) and (2).
