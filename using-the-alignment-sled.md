[< BACK](index.md)


# Part 1: Using the Alignment Sled 

## Detailed walk-through with prepared example files

Let's use [these already-prepared files (click to download)](tutorial-files.zip).  (Part 2 will discuss how to create the files.)  The bundle contains:

* **tuturial-print.pdf** — the file for printing.  The piece outlines have been expanded to allow for a little bit of error.
* **tutorial-print.jpg** — the same, in JPEG format.
* **tutorial-cut.svg** — the file for cutting.  This will need to be adjusted after some measurements are taken.
* **MAP-sled.svg** — the design for the disposable paper Measurement And Placement (MAP) sled.

### Materials needed:

_(See Q&A at the bottom for product recommendations.)_
* Photo printer & matte photo paper (or use a printing service)
* Photo mounting board
* Photo mounting adhesive
* Painter's tape
* Low-tack transfer tape
* Heavy (200gsm) letter-sized card stock
* Ruler with 1mm increments
* Paper slicer or Exacto knife

### Step 1: Lock down the crumb tray

Secure the crumb tray as described [here](https://community.glowforge.com/t/give-that-wiggly-gf-tray-the-boot/28329).

### Step 2: Attach a Three-Point positioning jig.

Solidly attach a Three-Point positioning jig (or equivalent) to the crumb tray. For example, I use [this one](https://community.glowforge.com/t/three-point-right-angle-positioning-jig/116003). We want a Three-Point jig, not a right angle jig, because the sheets of card stock won't always be perfectly square.

Position the Three-Point jig with its inside edges slightly outside (less than 5mm) the Glowforge cutting area. (This makes it possible to position the sled appropriately.)

![inside edges slightly outside (less than 5mm) the Glowforge cutting area](https://user-images.githubusercontent.com/25491795/210688015-519efa9d-a8bf-41c3-a1ee-a3fd7d0d39f9.png)

### Step 3: Decide whether to print your photo at home or to use a print service. 

Considerations are:

* De-masking ("weeding"): Masking is necessary for upside-down cuts. Photos from a print service are very easy to de-mask. If you use an inkjet printer at home, de-masking will be a challenge because transfer paper sticks like glue to inkjet photo paper. (You can weaken the transfer paper by repeated application to a piece of scrap photo paper, but it's a very fine line between "strong enough to do its job" and "weak enough to come off without tearing the photo", so I always end up with a few damaged pieces that need to be replaced. Fortunately, this method does allow you to cut replacement pieces!)

* Appearance of edges: It's nice if the puzzle pieces edges are less visible when viewing the completed puzzle. Inkjet-printed photos have an advantage here over lab-printed photos.

* Appearance of photo: I prefer matte paper. On inkjet printers you can get very nice high-contrast colors on matte paper. True matte photos printed at the lab will be lower-contrast. If you prefer glossy or satin, then it's not a problem.

* Durability: Lab-printed photos are more resistant to scuffing and scratches.

* Convenience: When you're first learning, expect to make mistakes and need to redo things. If ordering from a lab, order more than one copy to save turnaround time.

### Step 4: Print the example file (tutorial-print.pdf)

Print it on a letter-size sheet of matte photo paper.

Printing to the expected scale can be challenging. Some printers may crop or automatically resize the image. It's okay if you can't print at the original scale, as we'll work with the actual dimensions rather than the expected dimensions. Just make sure the black border is visible and not cropped, and is smaller than 261x198mm (to fit within the sled's measurement area). The example file is set up to accommodate up to 4% bleed or 6mm margins.

If you use a print service, use the .jpg file, and choose the option for no color correction.

### Step 5: Label the "Reference Corner".

Mark the bottom-left corner of the page (oriented in landscape position) as the Reference Corner.

### Step 6 Trim if necessary

Trim, if necessary, the *bottom and left* edges of the page (adjacent to the reference corner) so that there is less than 10mm between the black border and the edge of the page. (This is to avoid the photo print overhanging the sled.)  Don't lose the border. Example of trimmed print:

![trim](https://user-images.githubusercontent.com/25491795/210688247-f00a71af-b566-4b7e-8c37-0b5869eb1a27.jpg)

### Step 7: Mount the print

Mount it using your choice of backing board and adhesive. Make sure the board doesn't extend beyond the edge of the photo paper at the reference corner.

### Step 8: Determine cutting parameters and kerf adjustment

Using a separate scrap piece of identical photo paper and backing board, choose your cutting speed/power and run some [test cuts to decide how much kerf adjustment you want](https://community.glowforge.com/t/template-to-not-measure-the-kerf-test-directly-for-tightness-instead/116000). I've been using this strategy:

1. Choose a slower speed, like 170. (For better accuracy.)
2. Then choose the lowest power that cleanly cuts out all the pieces most of the time. (This is to reduce char, and also because weeding is easier if you don't cut all the way through the masking paper.)
3. Then make the test cuts, and choose a kerf adjustment that's about halfway between "the pieces just fall apart" and "the pieces are difficult to pull apart".

### Step 9: Mask the print

Mask it with transfer tape (low-tack if you can obtain it).

If you're using a lab-printed photo, this is straightforward.

If you are using an inkjet printer, it will be a little challenging.  The masking will stick to inkjet photo paper like glue.  Right now this is the best advice I can offer:

1. Start with matte inkjet photo paper, which tends to be a little less sticky than glossy.
2. Place the transfer paper sticky-side-up to the desk (taped down at the edges)
3. Around 10 times: stick a piece of cardstock to it (with gradually increasing pressure with the squeegee), then pull it off.
4. Around 10 times or more: stick a piece of spare photo paper to it (starting with very light squeegee pressure, increasing to medium), then pull it off.
5. Stop when it feels only slightly tacky. There’s a very fine line between “too strong to pull off” and “too weak to do its job”. It takes practice.
6. Apply the transfer paper to the photo, carefully avoiding introduction of bubbles, then lightly roll it down with a rubber roller (or you can manage with fingers). Again, the use of the right amount of force takes some practice.
7. Adjust your expectations.  Even with the above steps, you'll probably have some failed pieces (torn because the masking was too strong, or discolored because it was too weak.)  Fortunately, it's not difficult to cut replacement pieces.

### Step 10: Trim the masking

Use a [paper slicer](https://www.amazon.com/dp/B002OOVC84?ref=nb_sb_ss_w_as-reorder-t1_ypp_rep_k2_1_12&amp=&crid=2JCP8I7RSQRN7&sprefix=paper%2Bslicer&th=1) or exacto knife to trim the transfer paper so that the edge of the black border is left exposed. It should look like this:

![trimmed-mask](https://user-images.githubusercontent.com/25491795/210688378-0fe3b369-43ba-4c50-aea3-6799288e7f5b.jpeg)

### Step 11: Make an initial estimated measurement

Make an initial ("estimated") measurement with a ruler, to the outside edges of the black border, to the nearest millimeter.

![measurement-with-ruler](https://user-images.githubusercontent.com/25491795/210688432-ca255b57-335c-4aff-a812-575516a387a7.jpg)

### Step 12:  Alter the MAP sled template to match your estimated measurement.

Open the MAP-sled.svg design in the Glowforge interface. The diamond in the top-left corner, which you should find **centered** at (10mm,10mm), is the "Reference Corner".

Select the precision error gauge on the right-hand side. Move it **horizontally** so that it is **centered** at `x = (Estimated Width + 10mm)`.

Select the precision error gauge on the bottom. Move it **vertically** so that it is **centered** at `y = (Estimated Height + 10mm)`.

![sled-template-in-interface](https://user-images.githubusercontent.com/25491795/210688706-7771c9e2-f385-4e42-a20e-2f321bd050e3.jpg)

<p class="warning"><i>Glowforge interprets the SVG file assuming 96dpi.  <b>If you're not using a Glowforge</b>, you may need to adjust the scale.  The diamond in the corner should be centered at coordinates (10mm,10mm).  The height of the error gauge at the bottom (see picture above) should be 6mm.</i></p>

### Step 13:  Fix the cardstock in the jig

Place a sheet of heavy card stock in the Glowforge cutting area, snugly against the three-point jig

️Do not rush this step! Assure yourself that you can remove and replace the card stock in exactly the same position. 
Make sure the edge of the card stock is stopped against the three-point jig — not slipping underneath. If it keeps 
slipping under, try slightly bending up the edge of the paper.

Carefully, without moving it, tape down the corners with painter's tape.

<img width="432" alt="cutting sled" src="https://user-images.githubusercontent.com/25491795/210688594-18067b27-e461-4c8a-8753-d5f826872796.png">

### Step 14: Cut the MAP sled. 

For heavy card stock, I use speed 240, power 30. Don't use the highest speed, as it will be less accurate.

### Step 15: Align the sled to the photo.

Set the masked photo on the table, face up, with the reference corner at the bottom left.

Remove the cut sled from the Glowforge, and flip the sled upside-down, so that its reference corner is also at the bottom left.

Align the guide holes along the left and bottom edges of the sled to the left and bottom outside edges of the photo's black border.

![align the guide holes 2](https://user-images.githubusercontent.com/25491795/210688752-84ebd242-40f5-4558-90ef-e6a8e93338ae.jpg)

As best you can, get the edge of the border going right through the exact center of the guide holes. Then use painter's tape to tape the sled to the photo print, using the two round holes in the center area. After taping, double-check the alignment.

<img width="360" alt="aligned-magnified" src="https://user-images.githubusercontent.com/25491795/210688767-62b64c0a-6ce8-4538-b07c-1e8174a2bb93.png">

### Step 16: Make your precise measurement

Adjust your initial measurement using the error gauges in the sled. The error gauges, at the top and the right of the sled, let you tune your "estimated" dimensions to a precision of 0.1mm or better. The gauge measuring circles are arranged in increments of 0.1mm.

(Note, this is the step in which the photo's dimensions are directly mapped to Glowforge's coordinate system. The "real world" coordinate system, as defined by your favorite ruler, is actually irrelevant.)

![reading-error-gauges](https://user-images.githubusercontent.com/25491795/210688825-8453f7a4-9d8d-42f1-8e0e-365112f08608.jpg)

### Step 17:  Flip and place the photo for cutting.

Flip over the taped-together photo/sled assembly top-to-bottom, so that the reference corner is in the top left, and the photo is resting face-down on top of the sled.

Do not rush this step: Place the assembly back on the crumb tray against the Three-Point jig, with the sled in the exact same spot as before. The sled should be resting directly against the Three-Point jig. (If you can't do this because the photo is overhanging the sled, then you forgot to trim the photo. Start over at that step.)

Carefully pin it down without moving it.
<img width="380" alt="place-assembly-in-cutter" src="https://user-images.githubusercontent.com/25491795/210688853-15ee9987-05bf-47af-a8ca-ddc07e6220de.png">

### Step 18: Load the cutting file (tutorial-cut.svg) into your vector editor.

Make sure your editor is set to use units of millimeters, not pixels.

### Step 19: Adjust the cutting file dimensions

In the editor, "Select all" (rectangular boundary and pieces) and:

1. Flip the whole thing upside-down (Important: we're cutting upside down! After flipping, the reference corner is at the upper left).
2. Resize it to the corrected dimensions you measured using the error gauges. (Important: unlock the aspect ratio when doing this!)
3. Move it to position the top-left corner at (10mm, 10mm).

### Step 20:  Apply your kerf adjustment 

Apply the kerf adjustment to the pieces—but not the rectangular border!—including the four "canary pieces" in the corners.

- #### In Affinity Designer, it's the "Contour" tool
 - ![affinity-designer-contour](https://user-images.githubusercontent.com/25491795/210688868-6f2349bd-776f-441a-ba15-f6101c4c4ddf.jpg)
- #### In Inkscape, this is the "Outset" or "Dynamic Offset" tool
 - I'm not familiar with Inkscape, sorry
- #### In the Glowforge interface it's the "Create Outline" tool
 - I can't get this to work correctly.

### Step 21:  Load the design into Glowforge.

Save/export the design from your editor in the usual way, and upload it in the Glowforge interface. Verify the position and dimensions.

![verifying-cut-in-interface](https://user-images.githubusercontent.com/25491795/210688934-7f7d545d-c3ee-4857-955d-2ddc7affe377.jpg)

### Step 22 (optional but recommended):  Cut two canary pieces

Go ahead and cut two opposite "canary" pieces to check the alignment. Holding the sheet down in the GF so that it doesn't move, carefully pry out the canary pieces with a knife. You should get an accurately-cut red or green piece.

![canaries](https://user-images.githubusercontent.com/25491795/210688979-f3319a41-9619-4802-a875-96d20410e088.jpg)

### Step 23 Cut the pieces! 

Ignore (don't cut) the rectangular border.

### Step 24: Discard the paper sled

For the next job, print a new one. (This is because Glowforge's coordinates can drift over time.)

### Step 25: Remove ("weed") the masking paper and clean the edge char.

You can find advice elsewhere on this (in short, use Gorilla tape to pull off the masking paper, and tumble in Kosher salt to clean the char). But see later parts of the tutorial for my weeding trick.

### Step 26: Replace bad pieces

If there are any bad pieces (failed cut, face charring, photo torn during weeding), this method lets you cut individual replacements. Or, more simply, cut another copy of the whole puzzle to get a full inventory of replacement pieces for future copies.

Note that pieces cut from a separate sheet often won't be *perfectly* aligned, but they will usually be good enough for the puzzle player not to notice.

## Q & A

### Product recommendations?


* **Recommended**: Photo mounting board: this [1/16" plywood for mounting](https://www.amazon.com/gp/product/B08KPKCYDZ/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1) cuts cleanly with little char
* Photo paper: I prefer matte paper, as it gives a more elegant appearance, and de-masks more easily than glossy.  I'm using Canon double-sided matte paper, but I don't know its longevity.
* Transfer tape: I'm currently using [this](https://www.specialty-graphics.com/rtape-aplitape-4000-low-tack-tape-50-yd-roll/), but it still needs to be significantly weakened to use with inkjet photo paper.
* Photo mounting adhesive: there are options with pros and cons.
  * [3M 568 pressure-sensitive mounting adhesive](https://www.amazon.com/gp/product/B000JGQM1Q/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1): Cheaper than individual sheets, but a little difficult to use. This is the only option that claims to be "Photo Safe".
  * [These pressure-sensitive sheets](https://www.binding101.com/mounting-adhesive-sheets?sku=80PSMAS81211) are my favorite, but the website doesn't warn you if they're 4 weeks backordered!
  * [These instant-adhesive sheets](https://www.amazon.com/BENECREAT-Double-Sheets-8-3x11-5-Adhesive/dp/B0866XJ84S/ref=sxts_rp_s_a_1_0?content-id=amzn1.sym.eff26b9b-e255-411b-a40d-eccb21f93fe4%3Aamzn1.sym.eff26b9b-e255-411b-a40d-eccb21f93fe4&crid=3U74QPXJUGX4R&cv_ct_cx=double-sided%2Badhesive%2Bsheets&keywords=double-sided%2Badhesive%2Bsheets&pd_rd_i=B0866XJ84S&pd_rd_r=e78f8435-7dd9-404a-89a8-3c781455bc81&pd_rd_w=n4MNU&pd_rd_wg=QuFlA&pf_rd_p=eff26b9b-e255-411b-a40d-eccb21f93fe4&pf_rd_r=J9HMGCD3YHGDCTS78EYW&qid=1672700237&sprefix=double-sided%2Badhesive%2Bsheets%2Caps%2C130&sr=1-1-5985efba-8948-4f09-9122-d605505c9d1e&th=1) are cheaper but it's hard to avoid bubbles.
  * [Gorilla spray adhesive](https://www.amazon.com/gp/product/B08NTXD3XB/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1): Works but is very messy
* Heavy card stock: [these](https://www.amazon.com/gp/product/B08DDCR4NH/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1) are adequate. It's nice to have some with contrasting colors.
* **Recommended**: [Paper slicer](https://www.amazon.com/dp/B002OOVC84?ref=nb_sb_ss_w_as-reorder-t1_ypp_rep_k2_1_12&amp=&crid=2JCP8I7RSQRN7&sprefix=paper%2Bslicer&th=1): these are so useful that I have several around the house (office, kitchen, garage)
