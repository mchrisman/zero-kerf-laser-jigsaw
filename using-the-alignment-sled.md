[< BACK](index.md)


= Step-by-step walkthrough

Let's use these already-prepared files.  (Part 3 will discuss how to create the files.)  The attached .zip file contains:

	* tuturial-print.pdf — the file for printing.  The piece outlines have been expanded to allow for a little bit of error.
	* tutorial-print.jpg — the same, in JPEG format.
	•	tutorial-cut.svg — the file for cutting.  This will need to be adjusted after some measurements are taken.
	•	MAP-sled.svg — the design for the disposable paper Measurement And Placement (MAP) sled.

Materials needed:

	•	Photo printer (or use a printing service)
	•	Photo mounting board
	•	Photo mounting adhesive
	•	Painter's tape
	•	Transfer tape
	•	Heavy (200gsm) letter-sized card stock
	•	Ruler with 1mm increments
	•	Paper slicer or Exacto knife

Product links (I don't get a commission):
	•	Recommended: Photo mounting board: this 1/16" plywood for mounting cuts cleanly with little char
	•	Photo paper:  I prefer matte paper, as it gives a more elegant appearance, and de-masks more easily than glossy.
	•	Photo mounting adhesive:  there are options with pros and cons.
	•	3M 568 pressure-sensitive mounting adhesive: Cheaper than individual sheets, but a little difficult to use.  This is the only option that claims to be "Photo Safe".
	•	These pressure-sensitive sheets are my favorite, but the website doesn't warn you if they're 4 weeks backordered!
	•	These instant-adhesive sheets are cheaper but it's hard to avoid bubbles.
	•	Gorilla spray adhesive:  Works but is very messy
	•	Heavy card stock: these are adequate. It's nice to have some with contrasting colors.
	•	Recommended: Paper slicer:  these are so useful that I have several around the house (office, kitchen, garage)

Step 1:  Secure the crumb tray as described here.

Step 2:  Solidly attach a Three-Point positioning jig (or equivalent) to the crumb tray.  For example, I use this one. We want a Three-Point jig, not a right angle jig, because the sheets of card stock won't always be perfectly square.

Position the Three-Point jig with its inside edges slightly outside (less than 5mm) the Glowforge cutting area.  (This makes it possible to position the sled appropriately.)



Step 2:  Decide whether to print your photo at home or to use a print service.  Considerations are:

	•	De-masking ("weeding"):  Masking is necessary for upside-down cuts.  Photos from a print service are very easy to de-mask.  If you use an inkjet printer at home, de-masking will be a challenge because transfer paper sticks like glue to inkjet photo paper.  (You can weaken the transfer paper by repeated application to a piece of scrap photo paper, but it's a very fine line between "strong enough to do its job" and "weak enough to come off without tearing the photo", so I always end up with a few damaged pieces that need to be replaced.  Fortunately, this method does allow you to cut replacement pieces!)

	•	Appearance of edges:  It's nice if the puzzle pieces edges are less visible when viewing the completed puzzle.  Inkjet-printed photos have an advantage here over lab-printed photos.

	•	Appearance of photo:  I prefer matte paper.  On inkjet printers you can get very nice high-contrast colors on matte paper.  True matte photos printed at the lab will be lower-contrast.  If you prefer glossy or satin, then it's not a problem.

	•	Durability:  Lab-printed photos are more resistant to scuffing and scratches.

	•	Convenience:  When you're first learning, expect to make mistakes and need to redo things.  If ordering from a lab, order more than one copy to save turnaround time.

Step 3:  Print the example file (tutorial-print.pdf) on a letter-size sheet of matte photo paper.  

Printing to the expected scale can be challenging. Some printers may crop or automatically resize the image. It's okay if you can't print at the original scale, as we'll work with the actual dimensions rather than the expected dimensions. Just make sure the black border is visible and not cropped, and is smaller than 261x198mm (to fit within the sled's measurement area). The example file is set up to accommodate up to 4% bleed or 6mm margins.

If you use a print service, use the .jpg file, and choose the option for no color correction.

Step 4:  Label the bottom left corner of the page as the "Reference Corner".  

Step 5:  Trim, if necessary, the bottom and left edges of the page (adjacent to the reference corner) so that there is less than 10mm between the black border and the edge of the page.  But keep the border.  Example of trimmed print:


Step 4: Mount the print using your choice of backing board and adhesive.  Make sure the board doesn't overhang the photo paper at the reference corner.

Step 5: Using a separate scrap piece of identical photo paper and backing board, choose your cutting speed/power and run some test cuts to decide how much kerf adjustment you want.  I've been using this strategy:

	•	Choose a slower speed, like 170.  (For better accuracy.)
	•	Then choose the lowest power that cleanly cuts out 99% of the pieces.
	•	Then make the test cuts, and choose a kerf adjustment that's about halfway between "the pieces just fall apart" and "the pieces are difficult to pull apart".

Step 6: Mask the photo with transfer tape (low-tack if you can obtain it).  Note: transfer paper wants to stick like glue to inkjet photo paper!  You probably need to weaken it first, by repeatedly applying it and removing it to a piece of photo paper, with pressure increasing from light to medium.  It's something of an art to find the sweet spot between too weak and too strong.

Photos from printing services seem to be immune from this problem.

Step 7:  Use a paper slicer or exacto knife to trim the transfer paper so that the edge of the black border is left exposed.  It should look like this:


Step 8: Make an initial ("Estimated") measurement with a ruler, to the outside edges of the black border, to the nearest millimeter. 

Step 8: Place a sheet of heavy card stock snugly against the three-point jig.  

⚠️Do not rush this step!  Assure yourself that you can remove and replace the card stock in exactly the same position.  Make sure the edge of the card stock is stopped against the three-point jig --- not slipping underneath.  If it keeps slipping under, try slightly bending up the edge of the paper.

Carefully, without moving it, tape down the corners with painter's tape.



Step 9: Open the MAP-sled.svg design in the Glowforge interface.  The diamond in the top-left corner, centered at (10mm,10mm) is the "Reference Corner".

Select the precision error gauge on the right-hand side.  Move it horizontally so that it is 
centered at x = (Estimated Width + 10mm). 

Select the precision error gauge on the bottom.  Move it vertically so that it it is 
centered at y = (Estimated Height + 10mm).



Step 10:  Cut the MAP sled.   For heavy card stock, I use speed 240, power 30.  Don't use the highest speed as it will be less accurate.

Step 11:  Align the sled to the photo.

Set the masked photo on the table, face up, with the reference corner at the bottom left.  

Flip the sled upside-down, so that its reference corner is also at the bottom left.   

Align the guide holes along the left and bottom edges of the sled to the left and bottom outside edges of the photo's black border.   

As best you can, get the edge of the border going right through the exact center of the guide holes.  Then use painter's tape to tape the sled to the photo print, using the two round holes in the center area.  After taping, double-check the alignment.



Step 12:  Adjust your measurement using the error gauges in the sled.  The error gauges, at the top and the right of the sled, let you tune your "estimated" dimensions to a precision of 0.1mm or better.   The gauge measuring circles are arranged in increments of 0.1mm.

(Note, this is the step in which the photo's dimensions are directly mapped to Glowforge's coordinate system.  The "real world" coordinate system, as defined by your favorite ruler, is actually irrelevant.)



Step 13: Flip and place the photo for cutting.  

Flip over the taped-together sled+Photo assembly top-to-bottom, so that the reference corner is in the top left, and the photo is resting face-down on top of the sled.

👉 Do not rush this step:  Place the assembly back on the crumb tray against the Three-Point jig, with the sled in the exact same spot as before.  The sled should be resting directly against the Three-Point jig.  (If you can't do this because the photo is overhanging the sled, then you forgot to trim the photo.  Start over.)

Carefully pin it down without moving it.



Step 14:  Load the cutting file (tutorial-cut.svg) into your vector editor.  

(You can alternatively do the following edits in the Glowforge editor, but I prefer the vector editor.)

Step 15:  "Select all" (rectangular boundary and pieces) and:
  
	0.	Flip the whole thing upside-down (👉 important!  we're cutting upside down!  After flipping, the reference corner is at the upper left).
	0.	Resize it to the corrected dimensions you measured using the error gauges.  (Unlock the aspect ratio when doing this!)
	0.	Position it with the top-left corner at (10mm, 10mm).

Step 16:  Apply your kerf adjustment to the pieces—but not the rectangular border!—including the four "canary pieces" in the corners.  
	⁃	In Affinity Designer it's the "Contour" tool.  
	⁃	In Inkscape, this is the "Outset" or "Dynamic Offset" tool (but I'm not really familiar with Inkscape).
	⁃	In the Glowforge interface it's the "Create Outline" tool.

Step 17:  Load the design into Glowforge.  Verify the position and dimensions.



Step 18 (optional but recommended):  Go ahead and cut two opposite "canary" pieces to check the alignment.  Holding the sheet down in the GF so that it doesn't move, carefully pry out the canary pieces with a knife.   You should get an accurately-cut red or green piece. 


Step 19: Cut the pieces!  (Not the rectangular border.)


Step 19: Discard the paper sled; for the next job, print a new one.  (This is because Glowforge's coordinates can drift over time.)  

Step 20: Remove ("weed") the masking paper and clean the edge char.  

You can find advice elsewhere on this (in short, use Gorilla tape to pull off the masking paper, and tumble in Kosher salt to clean the char).  But see Part 4 of the tutorial for my weeding trick.  

Step 21: If there are any bad pieces (failed cut, face charring, photo torn during weeding), this method lets you cut individual replacements.   Or, more simply, cut another copy of the whole puzzle to get a full inventory of replacement pieces for future copies.

Pieces cut from a separate sheet often won't be perfectly aligned, but they will usually be good enough for the puzzle player not to notice.  



