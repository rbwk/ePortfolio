ASSETS FOLDER
=============

  photo.jpg    -> optional profile photo for the About page
                  (then edit about.html: replace the <div class="avatar">NC</div>
                   line with: <img class="avatar" src="assets/photo.jpg" alt="Nathan Chu">)

  portfolio/   -> co-op work samples shown on goals.html (Work Portfolio section)
  coursework/  -> COOP 2100 essays, papers, and video shown on portfolio.html


WORK PORTFOLIO (goals.html) - current state
-------------------------------------------
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
  If the video is over ~25 MB, link an unlisted YouTube upload instead of
  committing the file - GitHub rejects anything over 100 MB.


COURSEWORK (portfolio.html) - all six still to be added
--------------------------------------------------------
  coursework/vision-essay.pdf
  coursework/midpoint-journal.pdf
  coursework/why-me.mp4
  coursework/about-me-assignment.pdf
  coursework/values-assessment.pdf
  coursework/discussion-board.pdf

  Each card shows "PDF coming soon." until its file lands. The exact markup
  to paste in is in an HTML comment directly above each card.


BEFORE PUBLISHING ANY NEW PHOTO
-------------------------------
Check the frame for title blocks, drawing numbers, client names, site
addresses, signatures, and colleagues' faces. The original AECOM photo had a
consultant title block, a signature, and a registered engineer's number in
shot, so only a cropped version was published.

Phone photos can also carry GPS coordinates. Strip that before publishing.

Originals kept out of the repo are listed in .gitignore. They stay on this
machine and are never pushed.

Keep file names lowercase with no spaces (use-dashes-like-this.jpg) so links
work reliably once the site is live on GitHub Pages.
