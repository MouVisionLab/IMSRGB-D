# IMSRGB-D Dataset

This repository provides the IMSRGB-D dataset for stereo-depth-generation-based multi-scale RGB-D 3D perception of industrial targets.

IMSRGB-D is designed for industrial production-line perception, covering close-range manipulable objects and large-scale fixed infrastructure under challenging conditions such as reflection, occlusion, complex backgrounds, and object-scale variations.

## Dataset Overview

Each sample in IMSRGB-D contains:

* rectified left-view RGB image;
* rectified right-view image;
* stereo-derived disparity map aligned with the left-view RGB image;
* aligned instance mask annotation.

The right-view image is used for stereo disparity generation, while RGB-D perception models use the left-view RGB image and its corresponding disparity map as input.

## Target Categories

IMSRGB-D contains two target groups and six object categories.

### Manipulable Instance

* Tray

### Fixed Infrastructure

* CNC Machine
* Industrial Robot
* Material Stand
* Robot Control Cabinet
* Tool Cabinet

## Dataset Statistics

The complete IMSRGB-D dataset contains:

* 770 RGB-D samples;
* 3,255 object instances;
* 541 training samples;
* 99 validation samples;
* 130 test samples.

## Data Structure

Each sample is organized by a shared sample ID. The left-view image, right-view image, stereo-derived disparity map, instance mask, and annotation file with the same sample ID correspond to the same scene.

The current repository is organized as follows:

```text
IMSRGB-D/
├── README.md
├── dataset.yaml
├── release_plan.md
│
├── samples/
│   ├── images/
│   │   ├── left/
│   │   └── right/
│   ├── disparity/
│   ├── masks/
│   └── labels/
│
└── docs/
    ├── annotation_format.md
    ├── category_definition.md
    └── data_structure.md
```

The complete dataset will follow the same modality-based organization.

## Annotation Format

Instance annotations are aligned with the left-view RGB images and the corresponding stereo-derived disparity maps. The annotation format and representative sample files are provided in this repository.

## Release Plan

The complete IMSRGB-D dataset will be made publicly available upon acceptance of the paper. At this stage, this repository provides the dataset description, category definition, data organization, annotation format, and representative samples.

## License

The dataset is intended for academic research use. A formal license will be provided upon complete dataset release.
