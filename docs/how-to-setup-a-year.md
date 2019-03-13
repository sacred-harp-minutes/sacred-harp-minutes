# How to set up for a year worth of minutes

In the example below, we use the year _1957_. Substitute other years as appropriate.

1. Create a repository with the name `1957`
2. Copy ALTO, METS, OCR, PDF, SOURCE, TIFF for year into the repo, addn using `git add`, `git commit` and `git push`
3. Create small JPEG versions of the TIFF files in a directory called SMALL-JPEG

   On a Mac, this can be done with at the command line:
     - `cd TIFF`
     - `for i in *.tif; do sips -s format jpeg -s formatOptions 90 "${i}" --out "${i%tif}jpg"; done`
     - `mkdir ../SMALL-JPEG`
     - `mv *.jpg ../SMALL-JPEG`

4. Add, commit, push `SMALL-JEG` to the repository

5. Run the following script ... (TDB) to create issues

