# Structural Mean Modelling Mendelian Randomization (SMM-MR) Analysis

# Code for conducting Mendelian randomization (MR) analysis using g-estimation of structural mean models (SMM).

# This script uses an example based on the associated manuscript, which investigates the effects of childhood and adulthood adiposity on several later life outcomes.
# Polygenic risk scores (PRSs) were calculated using PLINK 2.00 based on SNPs identified in genome-wide association studies (GWAS) for childhood and adulthood adiposity.

# Univariable MR Analysis:
# In a univariable MR setting, PRSs were initially derived from SNPs meeting genome-wide significance for childhood adiposity (P ≤ 5×10^-8), excluding SNPs associated with adulthood adiposity at the same threshold. Similarly, PRSs for adulthood adiposity include SNPs meeting genome-wide significance for adulthood (P ≤ 5×10^-8), excluding SNPs associated with childhood adiposity. 
# Subsequent analyses used varying SNP-association thresholds as specified in the associated manuscript to explore the impact of instrument selection on period effect estimates. Each threshold was applied in turn to generate models with the respective PRS.

# Multivariable MR Analysis:
# We also applied SMMs in a multivariable framework to simultaneously estimate the effects of childhood and adulthood adiposity on outcomes.
# This approach estimates the controlled period effect of adiposity during a specific period by controlling for adiposity at a different life period. For this, PRSs are required for each life stage that do not exclude SNPs from other life stages.

