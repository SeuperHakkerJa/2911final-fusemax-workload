# FuseMax Workload

This is the ENGN2911 final project repository exploring FuseMax's effectiveness across different model sizes and context lengths.

Original paper repository: [micro24-fusemax-artifact](https://github.com/FPSG-UIUC/micro24-fusemax-artifact/tree/main)

## Overview

This project examines how FuseMax performance varies when scaling model parameters and input context lengths.

## Installation 
I have updated the docker config to support both ARM & X86 
Then follow the original [README](./FUSEMAXREADME.md) to set up the docker image.

## Results
![roofline1](workspace/notebooks/roofline_plots/roofline_plot_1_bert_baselines.jpeg)
![roofline2](workspace/notebooks/roofline_plots/roofline_plot_2_bert_varying_seq.jpeg)
![roofline3](workspace/notebooks/roofline_plots/roofline_plot_3_opt_pythia_components.jpeg)
![roofline4](workspace/notebooks/roofline_plots/roofline_plot_4_overall_comparison.jpeg)
![computeintensity](workspace/notebooks/oi_plots/bert_overall_oi_vs_context.jpeg)


# Reproducing results
1. BERT on fusemax with different level of optimization is saved in this [notebook](workspace/notebooks/figs.ipynb). (1k, and 4k length)
2. Pythia-14m on fusemax with different level of optimization is saved in this [notebook](workspace/notebooks/pythia.ipynb)
3. All theoretical roofline is saved in this [notebook](workspace/notebooks/theoreticalroofline.ipynb)
4. Operational intensity vs context length is saved in this [notebook](workspace/notebooks/workloadprogress.ipynb)



# Fibertree