# SlicerDMRI Tutorials

This repository holds the SlicerDMRI tutorial PDFs and source PowerPoint pptx files.

## Tutorial data

Data for each tutorial is attached to the [releases section of this repository](https://github.com/SlicerDMRI/tutorials/releases).
  - TODO

## Updating tutorials

- check out the repository (make sure to do this on a fast connection, because the repository is large due to images)
  - `git clone https://github.com/SlicerDMRI/tutorials`
    
    (note: add `--depth=1` for a [shallow clone](https://git-scm.com/docs/git-clone#git-clone---depthltdepthgt), to reduce transfer time if you are using
    git version >= 1.9)
    
  - copy the latest folder and rename based on target Slicer version. e.g.: `Slicer-4.8` --copy--> `Slicer-4.10`
  - edit the pptx files under `VERSION/ppt/*` as needed, and regenerate the PDF files
    - NOTE: please preserve the naming convention
  - commit the *new* files and `git push` back to GitHub
  
- to change the permalinks edit `_config.yml`, and update the version subdirectory (e.g.: `ver_subdir: Slicer-4.8`)

## Adding new tutorial
- follow the steps above but add a new PDF (and corresponding pptx) under the current version directory
- create a new directory with the permalink name (`NEW_DIRECTORY`)
- copy `dwi_converter/index.md` to `NEW_DIRECTORY/index.md`
- edit `NEW_DIRECTORY/index.md`
  - change the `redirect: DWIConverter.pdf` to the new PDF name
- Now `https://dmri.slicer.org/tutorials/NEW_DIRECTORY` should redirect to `https://dmri.slicer.org/tutorials/Slicer-4.8/NEW.pdf`
