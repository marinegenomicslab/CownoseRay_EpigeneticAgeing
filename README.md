# Weber et al. 2024 (Submitted to Scientific Reports)

Data and scripts/code associated with "Noninvasive, epigenetic age estimation in an elasmobranch, the cownose ray (*Rhinoptera bonasus*)" D. Nick Weber, Jennifer T. Wyffels, Chris Buckner, Robert George, F. Ed Latson, Veronique LePage, Kady Lyons, and David S. Portnoy. 2024. Submitted to Scientific Reports.

## Associated data can be found in the "Data" folder, including:
- "RADmeth_treated_filtered.zip" contains methylated and total read counts for all individuals and all CpG sites post-filtering for depth and coverage.
- "Metadata.csv" contains the metadata associated with all individuals included in the present study (including sample IDs and dates of birth).

## Associated code can be found in the "Scripts" folder, including:

- "ref_config.file" contains the code and parameters used to create a *de novo* reference genome for the cownose ray.
- "BAYES_GLM_wTissueSex_Days.r" contains code associated with the Bayesian GLM run with 4,000 warm-up/sampling iterations.
- "BAYES_GLM_wTissueSex_Days_50k.r" contains code associated with the Bayesian GLM run with 50,000 warm-up/sampling iterations.
- "95% CI's.Rmd" contains the code necessary to calculate 95% confidence intervals.
- The custom R script used to run elastic net regression involves the following scripts: "glmnet_loop.sh", "glmnet_prep.r", and "glmnet_loop.r". The script can be executed using the following code:
    glmnet_loop.sh input.csv ouput.txt iterations loci cpu_threads
