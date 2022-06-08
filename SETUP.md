#SETUP.md


## Steps taken to create the site.

use_github_action("bookdown")
renv::snapshot()
replaced the package installation bit in bookdown.yaml with an older one (still using renv) then it started working
no need to commit a gh-pages branch locally first
from Github repo enable pages


Chapter numbering.

0x0 to start a 'Part' add the Part header in the file
0x1 etc. within a part

## examples-mini
r scripts stored in their own folder
chapter file is created by : x-create-readme-book.r
add scripts & source x-create to update