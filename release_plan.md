# IMSRGB-D Release Plan

This document describes the release plan for the IMSRGB-D dataset.

## Current Release

At the current stage, this repository provides:

* dataset description;
* category definition;
* data organization;
* annotation format;
* representative sample data.

The representative samples are provided to illustrate the data format and modality alignment of IMSRGB-D.

## Complete Dataset

The complete IMSRGB-D dataset contains:

* 770 RGB-D samples;
* 3,255 object instances;
* 541 training samples;
* 99 validation samples;
* 130 test samples.

Each sample includes:

* rectified left-view RGB image;
* rectified right-view image;
* stereo-derived disparity map aligned with the left-view RGB image;
* aligned instance mask annotation.

## Release Schedule

The complete IMSRGB-D dataset will be made publicly available upon acceptance of the paper.

Before the complete release, the dataset will be checked and organized to ensure:

* consistent file naming;
* correct modality alignment;
* complete annotation files;
* train/validation/test split consistency;
* removal of sensitive or irrelevant information from industrial scenes.

## Data Access

The representative samples are available in this repository.

The complete dataset will be released through this repository or an external long-term storage platform, with the download link provided here after acceptance of the paper.

## Notes

The source code of the proposed model is not publicly released at this stage.
