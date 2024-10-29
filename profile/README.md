## Welcome to the HEFTIE project 🐘🧊

HEFTIE stands for "Handling Enormous Files from Tomography Imaging Experiments".
We are an EU funded project, which aims to:

> **develop a comprehensive digital textbook and new software tools for working with chunked 3D imaging datasets**

For a high level, public facing view of our project, see our [project page on the funder website](https://www.oscars-project.eu/projects/heftie-handling-enormous-files-tomographic-imaging-experiments).
This organisation README gives some more technical overview of what we are doing, targeted at existing chunked data communities so you can understand what we're up to.

### Who are we?

[@dstansby](https://github.com/dstansby/) is the project lead, and will be writing the digital texbook.
Python tools and benchmarking will be worked on by a couple of folks from UCL's [Centre for Advanced Research Computing.](https://www.ucl.ac.uk/advanced-research-computing)
Visualisation improvements will be done by scalableminds, led by [@normanrz](https://github.com/normanrz).


### What are we doing?

Our work is split into three work packages:

#### WP1: Digital textbook

The goal of this work package is to write a digital textbook for working with huge 3D imaging datasets.
This textbook wil explain how to work with huge 3D imaging datsets using modern data formats, focusing on explaining how chunked data formats work, and how to use them with practical examples.
Our examples will use the scientific Python stack with the [zarr](https://zarr.dev/) and [OME-zarr](https://ngff.openmicroscopy.org/index.html) data formats, and [dask](https://docs.dask.org/en/stable/) for chunked processing.
The draft chapter headings are:

1. Chunked dataset theory
2. Choosing parameters for chunked dataset creation
3. Converting between chunked datasets and 'traditional' file formats (e.g., TIFF, JPEG2000, NIfTI)
4. Downsampling chunked datasets
5. Working with remotely stored chunked datasets
6. Simple visualisation of chunked datasets
7. Simple analysis of chunked datasets

This is being developed at [HEFTIEProject/heftie-book](https://github.com/HEFTIEProject/heftie-textbook), and a live preview is available at https://heftie-textbook.readthedocs.io.

#### WP2: Tools and Benchmarks

The goals of this work package are to:
1. Develop a set of benchmarks to understand the best parameters for creating OME-zarr datasets.
2. Work on Python tools for working with OME-zarr datasets.

Instead of developing new tools, we want to help improve and fix existing tools.
Exactly what tools we work on will be guided by gaps we find when completing the digital textbook in WP1.

> [!TIP]
> **We would love feedback from the 3D imaging community on what tools they want to see developed!**

Current items on our TODO list include:
- Converting sub-volumes back and forth between 'tradditional' file formats (e.g., nifti, TIFF, JPEG)
- Caching remote data stores locally on disk
- Isotropically downsampling 3D images

But this is a tentative list - we would love to hear from you!
Please email [@dstansby](https://github.com/dstansby) with your thoughts or suggestions!

#### WP3: Visualisation and annotation

In this work package we will improve the existing open source [webknossos](https://webknossos.org) tool to add some more features for 3D datasets.
These improvements include:

- Region growing annotation tool in 3D
- Visualisation/interpolation/segmentation along tilted planes
- Expanding skeletons to segmentations
- Volume rendering in the 3D viewport

### How are we funded?

This project is funded by the [OSCARS project](https://oscars-project.eu/), which has received funding from the European Commission’s Horizon Europe Research and Innovation programme under grant agreement No. 101129751.

![OSCARS and EU logos](images/OSCARS-logo-EUflag.png)

<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
