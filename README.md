# Microfluidic Compression

Microfluidic compression experiments and image analysis for comparing the mechanical response of confined hydrogel cylinders.

This repository contains:

- the internship report describing the microfluidic device, experiments and results;
- a self-contained Jupyter notebook for tracking the cylinder, pusher and rigid wall;

## Analysis

Horizontal cylinder strain is measured directly from the tracked image edges:

\[
\varepsilon_x=\frac{D_0-D_x}{D_0},
\]

where \(D_0\) is the initial cylinder diameter and \(D_x\) is its horizontal width during compression.

The method provides relative comparisons between cylinders. It does not measure an absolute Young's modulus because the applied force is not calibrated.

## Usage

1. Preprocess and crop the microscopy videos in Fiji.
2. Place the processed TIFF stacks in one folder.
3. Set `INPUT_FOLDER` in the notebook.
4. Run all cells.
5. Review the diagnostic overlays before interpreting the results.

The notebook exports strain curves, quality-control information, frame-level measurements and comparison plots.

## Author

Mayad Mnif  
École Polytechnique — LadHyX, 2026
