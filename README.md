# OpenDIVE - BrainHack Vandy 2025
OpenDIVE (Open Diffusion Imaging Visualization for Everyone) is a command line interface tool for generating accessible, interpretable visualizations from diffusion MRI.

![Project description](https://github.com/MASILab/open_dive/blob/main/info_img.jpg)

Despite the prolific availability of software tools to visualize diffusion MRI data, there is no standardized visualization to summarize longitudinal changes. Similarly, the current standard of visualizations are not accessible to people with common forms of colorblindness. We propose a software package to both standardize and improve accessibility to representations of diffusion data. Aim 1: We will generate a standardized display for anatomical images to overlay the diffusion models based on user input. Aim 2: We compute bundle volume percent change over time, and given a specified color map, we display the tracks with the relevant color bar to summarize change over time. We can optimize this color map to be accessible for color-blind populations. 

The team will write documentation at the event. Installation and usage details will be available after 1/26/2025.

For FAQs related to diffusion MRI, see our diffusion FAQ issue (#4).

## Installation

TBD

## Usage

**Generic usage**
Initialize the conda or UV environment.
Run nifti2png directly as a command - do not run it with python.
By default, the tool will not display anything unless you use `--interactive`.
``nifti2png <arguments> path/to/file.nii.gz``

**Flags**
``--interactive`` : Will display a rotatable model of the slice in a window
``--value-range``: Requires two arguments for the min and max value range. The default is min-max of the entire data set, but this can be less useful in some cases. Refer to the color bar display in interactive mode to help define your specific range.
``--orientation`` or `-o`: The orientation of the slice of MRI image taken. Possible arguments are are `axial`, `saggital`, or `coronal`. 
``-slice``: Specifices the slice to display. Uses `m` to display the middle, or an integer (e.g. `10`) of the number of the slice


## Contributing

For details on contributing, please see [CONTRIBUTING.md](CONTRIBUTING.md)

## Contributors
- @saundersresearch
- @ElyssaMcMaster
- @neurolabusc
- @johaankjis
- @orekiwlg
- @mukhsadr
- @Beeper-Weepers

## License

[MIT](https://choosealicense.com/licenses/mit/)
