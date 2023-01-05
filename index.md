
# A technique for accurate laser cutting on upside-down digital prints (especially for making kerf-adjusted jigsaw puzzles)

This method uses a Measurement and Alignment (MAP) sled, the goal being "naked-eye perfect" cut alignment.

<p class="error"><b>This is not a beginner-level technique.</b> If you've never made a laser-cut jigsaw puzzle before, start with one of the many simple tutorials easily found on YouTube.</p>

<p class="info">Any comments or questions may be posted <a href="https://community.glowforge.com/t/kerf-adjusted-jigsaw-puzzles-tutorial/121437">in the Glowforge forum.</a></p>

<p class="warning">
<b>Fair warning:</b> I'm happy with the alignment technique.  But masking/de-masking inkjet photo paper is tricky; in spite of having practice, I usually have a few damaged pieces that need to be recut. Patience is required.</p>


## 90-second video overview

Start with this quick video: <!-- [https://www.youtube.com/watch?v=bI3UKxNdW8M](https://www.youtube.com/watch?v=bI3UKxNdW8M) -->

{% include youtube.html id="bI3UKxNdW8M" %}

## Tutorial

- [Part 1: Using the Alignment Sled](using-the-alignment-sled.md) — Detailed walk-through with prepared example files
- **Part 2: [forthcoming] Single-page puzzles** — How to create your own vector files
- **Part 3: [forthcoming] Masking and de-masking (weeding)** — Discussion; weeding trick
- **Part 4: [forthcoming] Multiple-page puzzles** — How to create your own vector files; how to mitigate relative error

## Q & A

#### Is "naked-eye perfect" alignment even possible?
The short answer: Just barely ... usually ... depending on the use case.  

I'll share the long answer later.  The TL;DR version:

* Jigsaw puzzle pieces should be relatively aligned within 0.2mm (depending on photo, resolution, piece size).
* Small puzzles cut from a single page appear perfect, because errors in adjacent pieces tend to cancel out.
* My own Glowforge is only accurate to 0.1mm (after compensating for scale and drift)
* My own error using this technique is usually less than 0.2mm.

#### Why cut upside-down?
Because in laser cutting, the kerf is always wider on top, narrower on the bottom.  For jigsaw puzzles, if you want the kerf reduced or eliminated on the front face, you need to cut it upside-down.

#### What is this good for?
* Making kerf-adjusted puzzles
* Accurately cutting out shapes from a picture
* Seamlessly joining halves of an oversized puzzle
* Cutting individual pieces (e.g. replacements)
* Scoring the back sides of prints, for origami fold lines.
