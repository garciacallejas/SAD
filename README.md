A repository for my study on species abundance distributions across trophic guilds (see my google scholar for the biorxiv preprint).

In this repository there are all the materials to fully replicate the study.

There are three types of scripts, I'll go one by one:

## 0 - load .Rprofile and create directory structure ##

Remember to install all the necessary packages and source the .Rprofile file, some of the packages are only available via devtools. In your project main folder, create a directory /results/images for the results of the scripts.

## 1 - Data preparation ##

Included in the repository are the GENTRY and MCDB datasets (/data/abundance datasets) as well as EltonTraits (/data/trophic_classification).
All these are also available in their respective repositories.

To prepare data for the analyses, run the following scripts:

#### SAD_trophic_guild_mammals_classification_3cat ####
#### SAD_site_data ####
#### SAD_species_data ####
#### SAD_abundances_data ####

These will classify all mammal species into trophic guilds, and will generate a single set of files (abundances, species, sites) with all entries.

## 2 - Theoretical model ##

Cohen's et al (2003) model is coded and evaluated through several scripts:

The first two generate predicted abundances and evaluate their goodness of fit for the tuesday lake dataset (also included in /data/abundance datasets):

#### SAD_cohen_tuesday_lake_predicted ####
#### SAD_cohen_tuesday_lake_fit ####

Then, the model itself is

#### SAD_cohen_abundances_model ####

Scripts for evaluating and printing the results are

#### SAD_cohen_model_results ####
#### SAD_cohen_model_plots ####

## 3 - Empirical datasets ##

With the files obtained at step 1, I calculate a set of metrics and evaluate them. Metrics are calculated with

#### SAD_empirical_data_metrics ####

and evaluated with

#### SAD_empirical_data_analyses ####

figures are produced in

#### SAD_empirical_metrics_plot ####
#### SAD_empirical_data_RAD_plot ####
#### SAD_empirical_data_proportions_dominance ####









