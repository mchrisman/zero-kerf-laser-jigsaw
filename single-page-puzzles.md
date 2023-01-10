[< BACK](index.md)

# Part 2: Single-Page Puzzles — Creating your own vector files

Here's how to create your own vector files for single-page kerf-adjusted jigsaw puzzles, such as the example used in [Part 1](using-the-alignment-sled.md).

## Materials

### Vector editor

I'll demonstrate using Affinity Designer, but Inkscape or other editors should work. The required features are common, though exact steps will vary:

* Filling a shape with an image.
* Offsetting the outline of a shape, nondestructively (reversibly)

### Files

* **The blank border template**: <a href="blank-border-template.svg" download>blank-border-template.svg (download)</a>
* **A jigsaw puzzle pattern** made up of 2D pieces, instead of 1D edges. You can [get some here](https://mchrisman.github.io/jigsawGenerator/).  (Hand-crafting your own is tricky, and isn't discussed in this tutorial.)
* **Your own picture image**.

## Step-by-step

### Companion video
👉I suggest following both video and text.

{% include youtube.html id="SXsY32mTGi4" %}


### Step 1: Clone the blank border template and add your picture

Make a copy of the blank border template <a href="blank-border-template.svg" download>(blank-border-template.svg)</a>.

Open the copy in the vector editor. Set the document size to 8.5"x11" (landscape orientation). "Select all", and scale and position the borders so that they fill the whole page with no margins (the edges of the color bars being at the edge of the page).

If your editor permits it, now "lock" the Print and Cut layers to prevent accidental editing of the borders.

Paste your photo into the middle of the page. Make it around 125mm high, to leave room for separating the pieces.

![snapshot-2-1](https://user-images.githubusercontent.com/25491795/211438751-1b0755e6-9a75-42d7-9a57-63e1287e7c82.jpg)

### Step 2: Getting a 2-D jigsaw template

We need a type of jigsaw puzzle template that consists of 2D pieces with closed boundaries, rather than the typical 1D edges.

[Click here to find a few hand-crafted 2D puzzle templates, as well as a random generator.](https://mchrisman.github.io/jigsawGenerator/)  

To fit on a single page, a 100-piece puzzle is about the right size.

### Step 3: Overlay the jigsaw template

Copy the jigsaw template into the file.

Make sure you are copying all of the individual pieces, **not** "embedding" the jigsaw template as an external resource. 

Resize and align the jigsaw pieces (as a group) to match the photo boundaries, but make it 1.0mm smaller than the photo in both dimensions. (We need a slight amount of padding to allow for error.)

![snapshot-2-2](https://user-images.githubusercontent.com/25491795/211438832-29f5c241-779e-4a11-a568-28baecd53e4a.jpg)

### Step 4: Set the picture as the fill background for each piece

👉 Easiest understood by watching the video.  

Every piece needs to be filled with the picture, specifically the exact same portion of the picture that's currently under that piece.  In Affinity Designer, the procedure is:

1. Select the photo image, and "Edit > Cut"
2. Select the first puzzle piece (any of them)
3. "Edit > Paste Inside"
4. Select the next puzzle piece with the mouse (or, "Select > Select Next").
5. Repeat (3) and (4) until you're done.

This is tedious because Affinity Designer doesn't have macro capability. But automation software like Keyboard Maestro for MacOS can make it easier.

If done correctly, you should now be able to move around the individual pieces with their background pictures.

![snapshot-2-3](https://user-images.githubusercontent.com/25491795/211438996-38301ef8-7229-475d-9b06-06f26becb26c.jpg)

### Step 5: Explode the puzzle

Move the pieces away from each other to leave 1.0mm of space between them. 

This is most easily done if you offset the piece outlines by 0.5mm.  (The background fills should stay fixed during this process.)  See the video.

Leave around 10mm space between the pieces and the black borders.

For best results, keep the pieces in the same positions relative to each other. If you must do some rearranging to make everything fit on the page, then

* Don't rotate the pieces!!
* Keep neighbors close together if possible

You can make an exception for parts of the image where alignment errors won't be noticeable, such as patches of sky. Rearrange those freely.

![snapshot-2-4](https://user-images.githubusercontent.com/25491795/211439025-53a22109-f353-422a-8b13-78c8994242d8.jpg)


### Step 6: Make "Print" and "Cut" versions of the pieces.

See the video for some tips on doing this efficiently. The important points are:
* Notice that the blank-border-template provided two layers, "Print" and "Cut". 
* Make two copies of the set of pieces. Put one copy in the Print layer, and one in the Cut layer. 
* For the pieces in the Print layer, **make sure that**
  * The picture fills are included
  * The outline offset are 0.5mm
  * The outline stroke are invisible.
* For the pieces in the Cut layer, **make sure that**
  * The picture fills are deleted
  * The solid-color backgrounds are deleted
  * The outline offset is 0mm
  * The outline stroke is visible.

You can refer back to the files from [Part 1](using-the-alignment-sled.md) ("tutorial-cut.svg" and "tutorial-print.jpg") for an example of the correct result.

### Step 7: Print and export

Now you're ready to 
* Print (or export to JPG or PDF) the "Print" layer.  Make sure the Cut layer is hidden when you do this!
* Export the "Cut" layer as your laser-cutting template.  Make sure the Print layer is hidden!

### Step 8: Finish making your puzzle

The steps for alignment and kerf adjustment were covered in [Part 1](using-the-alignment-sled.md).
