# Tierpsy-Tracking-Analysis
Scripts to analyse data produced by the tierpsy worm tracker.

## Track_images.ipynb

Takes raw trajectory data from tierpsy and plots images of tracks (individual and overlays).

Also puts data into a dataframe and adds strain information (for this to work the first 6 characters of each file name must be the strain name).

Option normalise tracks to the same starting point for overlay images, also can plot at least two variables in diff colours on top of eachother.

![image](https://user-images.githubusercontent.com/33955824/154326842-ffccc403-49e6-4a6e-ae20-0e29218485c6.png)

## 50th-simple-ttest-heatmap-plot.ipynb

To do a quick and simple analysis to find significantly different features in a small set of gentotypes

Generate a summary file from tierpsy data with trajectories ticked.
To this summary file add a coloum titled 'genotype'.
Save as a .csv and upload into script.

The script will use only the 50th percentile numbers for each feature and run mutliple individual t tests on each feature between two selected genotypes.

To make a heatmap of pvalues run all the desired comparisons between strains and save these files in a folder, these files will then be used to geneerate a p value heatmap.

At the end of the script there is also example plotting scripts in order to plot a few interesting features.
