# Generating Interactive Figures And Displays For Publications & Websites

- Friday March XX, 2024 YYY pm
- Location: Kline Tower -- TBD ()

This is a hands-on activity. **Bring your laptop and a dataset of your choice**, and leave with one (or more) interactive figures ready to submit with your next ApJ article.

## Installation instructions
All the examples that I show will be in Python. If you don't have Python, I recommend the Anaconda (miniconda) distribution. You can download it here: https://www.anaconda.com/products/individual (https://docs.conda.io/projects/miniconda/en/latest/)

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

I'm going to use Jupyter notebooks for the examples, but you can use all packages on the command line as well.


## Why interactive figures?
Astronomers have long used static figures and more recently movies in publications. However, in recent years, more and more journals allow interactive figures as electronic material which allow the reader to zoom, pan, click on objects in the scatter plot for more information, rotate 3D displays etc. This gives the reader of your article a way to explore more of the data you show, be more engaged, and understand your points better – hopefully leading to more citations!

Also, the same animations and interactive figures can be used on your own website, in talks, or to share with collaborators so they can easily zoom into a lightcurve, bin up a spectrum etc.

With the right plotting packages, making an interactive figure is no more complicated than making a pdf or png; I start off by showing a few examples in Python that I have personally used before (mpld3, bokeh, x3d) for those new to making interactive figures and then we’ll hack and make figures together. Bring your laptop and a dataset (table, image, catalog, …) you want to visualize and we’ll brainstorm if an interactive display is useful and what information it can add for the reader. If you’ve made a visualization like that before, bring it and teach us how!

## Examples of how plots might look like

- Optical design of the the Arcus satellite: https://space.mit.edu/home/guenther/ARCUS/3Dview.html
- Chen et al. (click on “start interaction”): https://iopscience.iop.org/article/10.3847/1538-4357/acb3a6#apjacb3a6f8 – I’ve made very similar plots with the same plotting package that they used myself, but my paper is still under review, so I don’t have link to share.
- Tully et al. (click on “start interaction”): https://iopscience.iop.org/article/10.3847/1538-4357/aceaf3#apjaceaf3f13 – This one looks cool!