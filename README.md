# Indexed Mapper

Source code for the method that is [described here](indexed_mapper.pdf). The method and results are ongoing research efforts! The actual source code is part of the [Mapper R package](https://github.com/peekxc/Mapper). Specifically, see the files: 

- src/MultiScale.xx
- src/GridIndex.xx
- R/MapperRef.R
- R/multiscale.R

## To reproduce 

To reproduce the experiments reported in the paper, do the following: 

1. Install the [Mapper package](https://github.com/peekxc/Mapper)
2. Install the dependencies 
	- R packages needed: data.table, ks, fastICA, RANN, reticulate, parallelDist
	- Python package needed: numpy, scikit-learn, umap-learn
3. Open the notebook `multiscale_benchmarks.Rmd` in Rstudio and click 'Run all'
	- The figures require ggplot2 and gridExtra to be installed

I use reticulate+miniconda to manage and load the python dependencies, and the path needs to be set to an appropriate conda environment with the above dependencies to run.