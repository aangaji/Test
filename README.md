# Test
This is a test repository


using:

*git config core.sparseCheckout true
*echo "folder 1/subfolder 1/\*/">>.git/info/sparse-checkout
*git pull origin master

only checks out subfolder 1. Changes in repo are still pulled and pushed, but dont appear on local repo if outside subfolder 1. More subdirectories can be added to *.git/info/sparse-checkout.*
For example: *.gitignore* file added on *Test/* level ignoring *\*.tex* files. The *.gitignore* file doesnt appear locally, but changes to *\*.tex* files are still ignored.
