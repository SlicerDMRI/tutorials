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
  
- edit the permalinks under slicerdmri.github.io
  - TODO
