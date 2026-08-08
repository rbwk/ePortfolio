ASSETS FOLDER
=============

  photo.jpg    -> optional profile photo for the About page
                  (then edit about.html: replace the <div class="avatar">NC</div>
                   line with: <img class="avatar" src="assets/photo.jpg" alt="Nathan Chu">)

  portfolio/   -> co-op work samples shown on goals.html (Work Portfolio section)
  coursework/  -> COOP 2100 papers and the About Me / Why Me video
  projects/    -> personal project images shown on portfolio.html

File names are lowercase with no spaces on purpose. GitHub Pages is
case-sensitive once the site is live, so WhymeVid.mp4 and whymevid.mp4 are two
different URLs. Keep to the convention and links stay reliable.


WORK PORTFOLIO (goals.html)
----------------------------
LIVE, already published:
  portfolio/cadimage.png            AutoCAD monorail / BMU layout
  portfolio/aecom-coordination.jpg  coordination photo, cropped
  portfolio/site-visit-1.jpg        site visit photo
  portfolio/site-visit-2.jpg        site visit photo

PERMANENTLY CONFIDENTIAL - leave these as-is:
  Method Statements & O&M Manuals
  Quotations & Tender Submissions
  Structural Design Calculations

  These three render a "Confidential - details available on request" box on
  purpose. That is the finished state, not an unfinished one. Do not drop
  files in for them unless the client has cleared that specific document.

STILL TO COME:
  A third site-visit photo, and the PWH video, if and when they are cleared.


ABOUT ME / WHY ME VIDEO - LIVE
-------------------------------
  coursework/why-me.mp4    (19 MB)

One file, used in two places:
  index.html      Introduction section, "Meet me" - satisfies the course
                  requirement to put the About Me video in the introduction
  portfolio.html  the "Why Me" coursework card

Both use preload="metadata", so a visitor downloads the 19 MB only if they
press play. Do not remove that attribute - without it every page load pulls
the whole file.

19 MB is comfortably inside GitHub's limits (it warns at 50 MB and rejects at
100 MB). If a future video is bigger, upload it to YouTube as UNLISTED and
swap the <video> block for an <iframe> pointing at youtube-nocookie.com.


PERSONAL PROJECT IMAGES - LIVE
-------------------------------
  projects/sim-shifter.jpeg   CAD assembly view of the shifter, with the joint
                              rotation limits annotated. This is a render, not
                              a photograph, and the alt text says so.
  projects/vex-robot.jpeg     the VEX competition robot on the field

If you ever shoot the physical shifter, add it alongside rather than replacing
this one - the CAD view and a real photo tell different halves of the story,
and the card text talks about iterating on the gate geometry.


COURSEWORK (portfolio.html)
-----------------------------
The self-assessments (DISC, values, About Me assignment, discussion boards)
are DELIBERATELY consolidated into one reflective card rather than posted as
six separate downloads. The course instructions warn that a dump of every
self-assessment scores badly. Do not split that card back out.

LIVE:
  coursework/midpoint-journal.pdf   linked from the Mid-Point Journal card

WITHHELD - needs a fix before it can go up:
  The vision essay is NOT published. Page 2 of the export carries the student
  ID line from the assignment cover page, which must not go on a public site,
  least of all one being handed round a class for peer review. (The number is
  deliberately not repeated here - this file is published too, and is readable
  at /assets/README.txt on the live site.) The original is parked at

      assets/vision-essay-HAS-STUDENT-ID-do-not-publish.pdf

  and is listed in .gitignore so it cannot be committed by accident.

  To publish it: delete the student ID line in the source document, export to
  assets/coursework/vision-essay.pdf, drop the .gitignore rule, and swap the
  "PDF coming soon." note on the Vision Essay card for
  <p><a href="assets/coursework/vision-essay.pdf">Read the essay (PDF) &rarr;</a></p>

  Everything else in that essay is fine - no contact details, nothing
  client-confidential.

One thing to note in the midpoint journal, your call rather than a blocker:
Week 3 records "two sick days". Normal in a journal handed to an instructor,
slightly more exposed on a public page an employer might read.


BEFORE PUBLISHING ANY NEW PHOTO
-------------------------------
Check the frame for title blocks, drawing numbers, client names, site
addresses, signatures, and colleagues' faces. The original AECOM photo had a
consultant title block, a signature, and a registered engineer's number in
shot, so only a cropped version was published.

Phone photos can also carry GPS coordinates. Strip that before publishing.

Originals kept out of the repo are listed in .gitignore. They stay on this
machine and are never pushed.
