# Generating Interactive Figures And Displays For Publications & Websites

- Tuesday, February 20, 2024 12n
- Location: Kline Tower -- Rm 501

This is a hands-on activity. **Bring your laptop and a dataset of your choice**, and leave with one (or more) interactive figures ready to submit with your next Journal article.

## Installation instructions
All the examples that will be in Python. If you don't have Python, I recommend the Anaconda (miniconda) distribution. You can download it here: https://www.anaconda.com/products/individual (https://docs.conda.io/projects/miniconda/en/latest/)

Once you have Anaconda (miniconda) installed, make a new environment for this workshop by opening a terminal and typing:
```
conda create -n interactive_figures python=3.11 jupyter numpy matplotlib astropy
```
which will install the packages used for the examples plus a few more. Then activate the environment by typing
```
conda activate interactive_figures
```
and install the plotting packages:

```
pip install mpld3
pip install bokeh
pip install x3d
pip install plotly
```
other packages used in this Tutorial:
```
pip install pyvo
pip install mocpy
pip install ipyaladin
```

We will be using Jupyter notebooks for the examples, but you can use all packages on the command line as well.


## Why interactive figures?
Astronomers have long used static figures and more recently (since 1995!) movies in publications. However, in recent years, more and more journals allow interactive figures as electronic material that allow the reader to zoom, pan, click on objects in the scatter plot for more information, rotate 3D displays etc. The AAS Journals have supported inline (HTML) interactive graphics since 2014; authors have published nearly 200 such figures so far. Interactive Figures give the reader of your article a way to explore more of the data you show, be more engaged, and understand your points better – hopefully leading to more citations!

Also, the same animations and interactive figures can be used on your own website, in talks, or to share with collaborators so they can easily zoom into a lightcurve, bin up a spectrum etc.

With the right plotting packages, making an interactive figure is no more complicated than making a pdf or png; I will start by introducing a few examples, borrowed from Moritz Günther or authors submitting to the AAS Journals, then we’ll hack and make figures together. Bring your laptop and a dataset (table, image, catalog, …) you want to visualize, and we’ll brainstorm if an interactive display is useful and what information it can add for the reader. If you’ve made a visualization like that before, bring it and teach us how!

## General Steps/Workflow

1. Select a dataset used in a bunch related graphs for a manuscript. Such a dataset makes for good, first example because you find yourself often "reprojecting" the same data different ways for multiple "static" figures in your manuscript;
2. Use a toolkit to create a multi-view or interactive view of that dataset;
3. Package the graphic up for submission to a Journal;
4. Prepare a separate package of data, notebooks and scripts that document and explain how the graphic was created.
5. Submit the graphic and this "data behind the figure" to the Journal.

## Examples of how plots might look like

- You can find all the Interactive Graphics in the AAS Journals using the AstroExplorer (select "Interactive Figures" from the facets on the left): https://www.astroexplorer.org/
- X3D examples:
    - Optical design of the the Arcus satellite: https://space.mit.edu/home/guenther/ARCUS/3Dview.html
    - 3D mesh models of PNs in Danehkar (2022) [Figure 5, click on "start interaction"]: https://doi.org/10.3847/1538-4365/ac5cca
    - 3D visualization of outflows traced by 12CO in Lu et al. (2018) [Figures 12-24]: https://doi.org/10.3847/1538-4357/aaad11 (using tdviz:https://github.com/xinglunju/tdviz)
- Bokeh examples:
    - Chen et al. 2023 [Figures 8-11, (click on “start interaction”)]: https://doi.org/10.3847/1538-4357/acb3a6
- Plotly Examples:
    - Distribution of the C18O (1–0) velocity centroids of 30 identified filaments, Yoo et al. (2023) [Figure 9]: https://doi.org/10.3847/1538-4357/acf8c2
- Tully et al. (click on “start interaction”): https://iopscience.iop.org/article/10.3847/1538-4357/aceaf3#apjaceaf3f13 – These are pretty cool. They use SketchFab to host the 3D elements for the interactive graphic. We won't talk about SketchFab graphics today.

## Resources

- [plotly](https://plotly.com/python/getting-started/)
- [bokeh](https://docs.bokeh.org/en/latest/docs/first_steps.html#first-steps)
- [ipyaladin](https://github.com/cds-astro/ipyaladin)


## Articles / Data used

- Gaia-based Isochronal, Kinematic, and Spatial Analysis of the epsilon Cha Association, [D. Annie Dickson-Vandervelde et al 2021 AJ 161 87](https://doi.org/10.3847/1538-3881/abd0fd) 
    - Using Vizier data extracted from the article: [J/AJ/161/87](https://doi.org/10.26093/cds/vizier.51610087) in FITS format
- The Lyα Reference Sample. XIV. Lyα Imaging of 45 Low-redshift Star-forming Galaxies and Inferences on Global Emission, [Jens Melinder et al 2023 ApJS 266 15](https://doi.org/10.3847/1538-4365/acc2b8) _with six machine-readable tables in the article_.
    - Vizier version (w/Notebook) [vizier:J/ApJS/266/15](https://doi.org/10.26093/cds/vizier.22660015)
- The Swift Deep Galactic Plane Survey (DGPS) Phase I Catalog, [B. O'Connor et al 2023 ApJS 269 49](https://doi.org/10.3847/1538-4365/ad0228), _with two machine-readable tables in the article_

