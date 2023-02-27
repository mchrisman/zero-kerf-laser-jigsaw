
{% include analytics.html %}

[< BACK TO  TABLE OF CONTENTS](index.md)

# Part 4: Multi-page puzzles

When making a puzzle that's too large to fit on one page, obviously you can just divide up the pieces into multiple pages ... but we have to think about alignment error.

Adjacent pieces cut from the same page will have perfect alignment (relative to each other).  Pieces cut from different pages may not be perfectly aligned.

## How much error is typical?  How much is tolerable?

For the method described in this tutorial, I expect a cutting accuracy of 0.1–0.2mm, depending on the condition of your Glowforge.  In cutting two pages, the relative error can be double that, but usually it's within 0.2mm.  That's barely tolerable (see Q&A below), so we want to mitigate the error.

## How to mitigate the error

For most multi-page puzzles, you can get a good result by simply dividing up the puzzle strategically.  Keep in mind that a pair of adjacent pieces may be 

* **"Inseparable"** :  Misalignment will be noticed.  The cut goes through straight lines or edges, important details, people's faces, the main subject of the image.

* **"Separable"**:  Misalignment will be invisible or appear normal.  The cut goes through patches of open sky, fuzzy or grainy areas, grass, irregular jagged and broken lines or edges.

(Those aren't black-and-white categories, of course.)  Then, as much as possible:

1. By default, keep all of the pieces in the same relative position and orientation.  Don't rotate them.
2. For "inseparable" pairs, follow rule #1 strictly.
3. Never split "inseparable" pairs apart onto separate pages.  If this is impossible, find the split that will be the least noticeable.
4. Lay out your "separable" pieces last.  Because they can be moved around and rotated freely, you can use them to balance the number of pieces between pages, and to get everything to fit on the page.

Here's an example of what I did for this puzzle:

![Pasted Graphic](https://user-images.githubusercontent.com/25491795/216195092-c2ef3849-3992-4b43-b893-98ee23ae7390.png)

I broke the puzzle into four pages of equal area,

![Pasted Graphic 3](https://user-images.githubusercontent.com/25491795/216195148-89d33218-13f3-4cb8-82db-e679c0c2ec48.png)

Then altered the split lines to avoid the ships, masts and sail lines (I couldn't entirely avoid splitting the horizon line),

![Pasted Graphic 4](https://user-images.githubusercontent.com/25491795/216195206-ab567c66-cb5f-4423-8d85-48c6bfd984ba.png)

and moved some unimportant pieces of sky around to re-balance the pages

![Pasted Graphic 5](https://user-images.githubusercontent.com/25491795/216195269-649f39b8-917d-4dde-b8b3-17720dda3107.png)

To place the pieces onto the actual pages, I started with the important "inseparable" pieces, keeping adjacent pieces in their original relative positions,

![Pasted Graphic 6](https://user-images.githubusercontent.com/25491795/216195336-ebe2adfb-1df1-4ee6-a71c-9ef41b76c4e8.png)

Then filled in the "nooks and crannies" with the freely-movable "separable" pieces.

![Pasted Graphic 9](https://user-images.githubusercontent.com/25491795/216195394-a45a3840-6893-451c-8d06-0572a7d00c74.png)

And that's ready to go!

## Printing

When printing the photos, or sending them to the photo lab, make sure the file for every page has the same dimensions and resolution.  

For the photo lab, don't choose the "color correction" option.  For inkjet printing, disable any automatic color correction in your printer/driver settings.  You don't want the algorithms applying slightly different color profiles to the two pages!

When you have the prints, hold them next to each other and compare the color bars.  They should be identical.

## Dealing with mismatched page scales

Photo printers aren't perfect.  As you perform the measurement/alignment procedure for each page, you may find that the different pages don't quite match each other in dimensions.

Mismatches of less than 0.2mm are very common and may be ignored; just process each page individually.   However, if there is a significant difference in dimensions between pages, such as a 2mm difference, it may affect how the puzzle pieces fit together.  (What's a "significant" difference?  Not sure. Best guess, around 1mm.)

This problem is rare when all pages are printed together in one batch. If it does occur, the cut file can be adjusted to compensate:

1. Prepare the kerf-adjusted cut files, one per page, as usual.
2. Make note of the ratios in each dimension; for example:
```
Page 1 printed image size = (256.3mm, 195.2mm)
Page 2 printed image size  = (256.9mm, 194.0mm)
X-ratio = 256.9/256.3 = 1.0023
Y-ratio =  194.0/195.2 = 0.9938
```
3. Edit the cut file for Page 2, and expand/shrink each puzzle piece by that ratio.  (**Important:** Multiply, don't add.)  This puts Page 2's pieces at the same scale as Page 1's pieces. (**Important:** alter each piece individually, relative to its midpoint.  Don't alter them as a group, because you don't want them to move.  In Affinity Designer, you can do this in one step using the "Transform Objects Individually" feature.)

Repeat for pages 3, 4, etc., bringing them into the same scale as Page 1.

[< BACK TO  TABLE OF CONTENTS](index.md)

## Q&A

### How much accuracy is actually required?

This is a hard question because it depends on 

* The resolution of the photo in its printed size.  Lower-resolution photos don't need as much accuracy.
* The size of the pieces.  A small misalignment will be more obvious in a 1/2" puzzle piece vs. a 1" puzzle piece.
* The presence of sharp edges and straight lines in the photo, especially at focal points such as people's faces or the picture's primary subject.  It's easy to spot a misalignment there.

As a rule of thumb, you probably want an error of 0.2mm (0.01") or less. Here's a picture showing errors of different sizes:

![Perfect alignment](https://user-images.githubusercontent.com/25491795/216194898-4ab0f16d-cf71-491e-b273-213850b6cf0c.jpg)
