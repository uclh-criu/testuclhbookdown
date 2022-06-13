#SETUP.md

## on update
add any packages to DESCRIPTION
renv::snapshot()
beware that seems that there are a load of packages incl. tidyverse, googlesheets etc. in the renv lockfile that aren't used in the book pages - maybe some are from the slides and don't need to be there.
This which is supposed to just query DESCRIPTION excludes them.
renv::snapshot(type="explicit")

## Steps taken to create the site.

use_github_action("bookdown")
renv::snapshot()
replaced the package installation bit in bookdown.yaml with an older one (still using renv) then it started working
no need to commit a gh-pages branch locally first
from Github repo enable pages
added DESCRIPTION file for dependencies

Chapter numbering.

0x0 to start a 'Part' add the Part header in the file
0x1 etc. within a part

## examples-mini
r scripts stored in their own folder
chapter file is created by : x-create-readme-book.r
add scripts & source x-create to update