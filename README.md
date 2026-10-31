# wychoi.com — public build log
The source for the site at wychoi.com is private. This repository is the public build log and the source of the Workbench card that appears on the site. It contains no site source.


## Build notes
The Workbench card is defined in workbench.md.
The repo About description and topics supply the card's front summary and tags.
The back uses the first ## section for What it is and two short notes for the hardest part and the main lesson.
The card flips on four axes. Four stacked layers share the same state; only the visible layer is painted and animated. The return switches to a different layer, so it lands on a different axis.
The résumé PDF is generated at build time, not at request time.
Live site
wychoi.com
