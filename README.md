# social_rent_rdd
Social rent regression discontinuity design.

# description of repo
This repo provides all scripts and data to reproduce the analysis on the effects of Homes England grant funding on social rented housing delivery within local authorities.

# script running order
First, run **01_sdr_and_voa_dataset.R** to create the affordability gap variable - that is used to calculate the treatment - from the SDR, ONS and VOA data. This step can be avoided by downloading the **rent_gap_full.Rdata** file, which is the output of this script, and is loaded in the subsequent script.

Second, run **03_social_rent_rdd_markdown.Rmd** to run the regression discontinuity design analysis. This markdown produces a github_document entitled **03_social_rent_rdd_markdown.md**, which is already uploaded to this repo. So if you wish to skip running the markdown, and simply view the output, you can do so by opening **03_social_rent_rdd_markdown.md**.

# data
All necessary datasets are uploaded as either xlsx or csv files to the repo. Hyperlinks to their original locations are included in **03_social_rent_rdd_markdown.Rmd**. 

As mentioned, the necessary SDR, VOA and ONS data is consolidated into the **rent_gap_full.Rdata** file, so the **01_sdr_and_voa_dataset.R** script can be skipped if preferred.

# package pre-requisites
The *pacman* package should be installed prior to running all scripts. Otherwise, all necessary packages are installed and/or loaded within the scripts.
