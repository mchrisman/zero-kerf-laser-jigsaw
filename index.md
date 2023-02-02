
# A technique for accurate laser cutting on upside-down digital prints.

Among other applications, you can use this to make **zero-kerf photo jigsaw puzzles**.

<p class="error"><b>Beginners:</b> If you've never made a laser-cut jigsaw puzzle before, learn the easy way first. There are a lot of tutorials on YouTube.<br/><br/><b>Experienced puzzle makers:</b> Eliminating kerf is straightforward but requires more effort.  Larger puzzles are expensive because you need multiple pages.</p>

<p class="info">Any comments or questions may be posted <a href="https://community.glowforge.com/t/kerf-adjusted-jigsaw-puzzles-tutorial/121437">in the Glowforge forum.</a></p>

## 90-second video overview

This quick video shows the essence of the precision cutting technique, which can often achive "naked-eye perfect" alignment.  (This is also the companion video for Part 1 of the tutorial.)

{% include youtube.html id="bI3UKxNdW8M" %}

## Tutorial

- [Part 1: Precision Cuts Using the Alignment Sled](using-the-alignment-sled.md) — Learn to make precision upside-down photo cuts.  Detailed walk-through for an example application (making a kerf-adjusted jigsaw puzzle, with pre-prepared files).
- [Part 2: Setting up files for single-page puzzles](single-page-puzzles.md) — Learn to create vector files for a small zero-kerf jigsaw puzzle.
- [Part 3: Masking and Weeding](masking-and-weeding.md) — Discussion; weeding trick
- [Part 4: Multi-page puzzles](multipage-puzzles.md) — How to divide the puzzle; how to mitigate relative error

## Supplementary

[Jigsaw template generator for 2D pieces instead of 1D edges](https://mchrisman.github.io/jigsawGenerator/)

## Gallery

* [Micro zero-kerf puzzles](https://community.glowforge.com/t/christmas-russian-doll-jigsaw-puzzles-micro-puzzles/121318)
* [Oversized zero-kerf puzzle](https://community.glowforge.com/t/picture-jigsaw-puzzles-with-kerf-eliminated-snugly-fitting/121229)

## Q & A


#### Is "naked-eye perfect" alignment even possible?
The short answer: Just barely ... usually ... depending on the use case.

* Jigsaw puzzle pieces should be relatively aligned within 0.2mm (depending on photo, resolution, piece size, audience).
* Small puzzles cut from a single page appear perfect, because errors in adjacent pieces tend to cancel out.
* My own Glowforge is only accurate to 0.1mm (after compensating for scale and drift)
* I can usually place cuts with error under 0.2mm.

#### Why cut upside-down?
Because in laser cutting, the kerf is always wider on top, narrower on the bottom.  For jigsaw puzzles, if you want the kerf reduced or eliminated on the front face, you need to cut it upside-down.

#### What is this good for?
* Making zero-kerf puzzles
* Accurately cutting out shapes from a picture
* Seamlessly joining halves of an oversized puzzle
* Cutting individual pieces (e.g. replacements)
* Scoring the back sides of prints, for origami fold lines.

#### What is the MAP sled solving (that can't be solved with a ruler and stationary jig)?

It compensates for these sources of error, _any_ of which can be greater than our target accuracy of 0.2mm:

1. The **position of the printed image** on the page isn't precise.
2. The **size of the printed image** on the page isn't precise.
3. The **printed image may not be precisely parallel** to the page edges (which themselves may not be precisely at right angles).
4. **Glowforge's coordinate system can shift** every time it recalibrates itself, and can also drift over time.
6. **Glowforge's coordinate system can be slightly out of scale**, relative to the "real-world" distances defined by your favorite precision ruler.  (For me the difference is about 0.1mm per 250mm.)  

The sled is designed to directly align the printed image's boundaries with Glowforge's coordinate system, without the intermediate step of going through the (irrelevant) real-world coordinate system.  The sled is disposable and generally single-use because of (4).
