# How to set up for a year worth of minutes

In the example below, we use the year _1957_. Substitute other years as appropriate.

1. Create a repository with the name `1957`
2. Create small JPEG versions of the TIFF files in a directory called SMALL-JPEG

   On a Mac, this can be done with at the command line:
     - `cd TIFF`
     - `for i in *.tif; do sips -s format jpeg -s formatOptions 90 "${i}" --out "${i%tif}jpg"; done`
     - `mkdir ../BW-JPEG`
     - `mv *.jpg ../BW-JPEG`

2. Retitle folders what they should be:
   - to OCR-A and CORRECTED-A
   - to OCR-B and CORRECTED-B
   - to COLOR-JPEG
   
3. Copy these for year into the repo, addn using `git add`, `git commit` and `git push`


4. Run the following script ... (TDB) to create issues

