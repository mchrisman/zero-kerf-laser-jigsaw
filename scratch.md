
<script async src="https://www.googletagmanager.com/gtag/js?id=G-RMNG6FJDBG"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'G-RMNG6FJDBG');
</script>


<p> A non-script... </p>

#### What is the MAP sled solving (that can't be solved with a ruler and stationary jig)?

It compensates for:

1. Glowforge's coordinate system origin can shift every time it recalibrates itself (millimeter-scale errors can happen)
2. Glowforge's coordinate system origin can drift over time (sub-millimeter-scale errors are typical)
3. Glowforge's coordinate system can be slightly out of scale (relative to the "real-world" distances defined by your favorite ruler).
4. The **position** and **size** of the printed image on the page isn't predictable. (Large errors are seen due to bleed or driver defaults. From page to page, smaller millimeter-scale differences of position and sub-millimeter-scale differences of size are typical.)

The sled is designed to directly align the printed image's boundaries with Glowforge's coordinate system, without the intermediate step of going through the (irrelevant) real-world coordinate system.  The sled is disposable and generally single-use because of (1) and (2).

#### What is "kerf" and "kerf-adjusted"?

"Kerf" refers to the gap or space created when a laser cutter cuts through material. "Kerf adjustment" refers to slightly expanding the outline of puzzle pieces to make them fit more closely together and eliminate the gap created by the laser cutter. This can only be done by cutting the pieces individually.



## Supplemental

-  **Discussion of accuracy [forthcoming]** — How accurate do you need to be? How accurate **can** you be?



