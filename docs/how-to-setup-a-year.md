# How to set up for a year worth of minutes

In the example below, we use the year _1957_. Substitute other years as appropriate.

1. Upload the entire `1957` directory on your local machine as a subdirectory of the `sacred-harp-minutes-preservation` repository. See [instructions](https://github.com/sacred-harp-minutes/standard-git-commands).

2. Create a new repository with the name `1957`

3. Create small JPEG versions of the TIFF files in a directory called `JPEG-BW`

   On a Mac, this can be done at the command line:
     - `cd TIFF`
     - `for i in *.tif; do sips -s format jpeg -s formatOptions 90 "${i}" --out "${i%tif}jpg"; done`
     - `mkdir ../JPEG-BW`
     - `mv *.jpg ../JPEG-BW`

4. Retitle folders as follows so that their contents are easy to understand
   - `OCR` to `OCR-A`
   - `OCROPUS` to `OCR-O`
   - `PDF` to `PDF-COLOR`
   
5. Follow steps 1 and 2 in these [instructions](https://github.com/sacred-harp-minutes/standard-git-commands/blob/master/README.md), then move `JPEG-BW` and the three just-retitled folders for the year into the repo using `git add`, `git commit` and `git push` as described in step 6 of the instructions.

6. Run the following script ... (TDB) to create issues
