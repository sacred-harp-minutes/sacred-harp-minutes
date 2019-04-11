# How to set up for a year worth of minutes

In the example below, we use the year _1957_. Substitute other years as appropriate.

1. Upload the entire `1957` directory on your local machine as a subdirectory of the `sacred-harp-minutes-preservation` repository.

2. Create a new repository with the name `1957`

3. Create small JPEG versions of the TIFF files in a directory called SMALL-JPEG

   On a Mac, this can be done with at the command line:
     - `cd TIFF`
     - `for i in *.tif; do sips -s format jpeg -s formatOptions 90 "${i}" --out "${i%tif}jpg"; done`
     - `mkdir ../BW-JPEG`
     - `mv *.jpg ../BW-JPEG`

4. Retitle folders as follows so that their contents are easy to understand
   - `OCR` to OCR-A and CORRECTED-A
   - `Ocropus` to OCR-B and CORRECTED-B
   - `SOURCE` to COLOR-JPEG
   
5. Copy these plus `SMALL-JPEG` for year into the repo using `git add`, `git commit` and `git push`

6. Run the following script ... (TDB) to create issues
