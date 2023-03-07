# Yale Workshop
This repository contains data and code associated with a workshop at Yale on March 10, 2023. Most of this material was originally developed for a workshop at the International Statistical Ecology Conference in Cape Town, South Africa that was held in July of 2022. That workshop was titled *Advances in quantifying space-use and habitat-selection of animals*.

**Contributers**: 

- John Fieberg, University of Minnesota, USA 
- Johannes Signer, University of Göttingen, Germany
- Brian Smith, Utah State University, USA, 
- Stefanie Muff, Norwegian University of Science and Technology, Norway.
 
**Integrated Step-Selection Functions (iSSFs)**: offer a simple framework for simultaneous modeling animal movement and habitat selection processes using conditional logistic regression (Avgar et al. 2016, Fieberg et al. 2021). These models allow one to relax the assumption that movement characteristics (i.e. step lengths and turn angles) are independent of habitat features.
 

For this workshop, John will demonstrate how to implement an integrated step-selection analysis (iSSA) using the amt package and simulated data for a single focal individual (`amt_demo_iSSF.R`).  Johannes will also demonstrate methods for simulating movements using fitted models.  

**Coded examples**

- `amt_demo_iSSF.R` = demonstration of how to conduct an integrated step-selection analysis using the `amt` package [Code written by Brian Smith, with minor adjustments by John Fieberg]

- `two_step_approach.R`: demonstrates how one can easily fit models to multiple individuals and then use a bootstrap for population-level inferences (Signer et al. 2019).  This approach is then compared to a mixed-effect SSA. [Code written by Johannes Signer and John Fieberg]

- `Otters_SSF.R`: illustrates methods for fitting models to multiple individuals, using random effects to capture among animal variability in their habitat selection parameters (Muff et al. 2021). [Code written by Steffi Muff with minor adjustments made by John Fieberg]
 
  
## Software

### R and RStudio

Please make sure you have [installed `R` version >4.2.0](https://cran.r-project.org/). We also recommend the latest version of [RStudio Desktop](https://www.rstudio.com/products/rstudio/download/). 

<!---
To build packages from source, you will need additional build tools; see details [here for Windows](https://cran.r-project.org/bin/windows/Rtools/) or [here for macOS](https://mac.r-project.org/tools/). 

*Note* that if you are upgrading to R 4.2 from a previous version on Windows, you will need RTools 4.2 as well. Your previous RTools installation will not be sufficient.
--->

### R Packages
<!---
*The script* `packages.R` *in this repository can help you install and/or update the packages required for this workshop.*
--->

We will be highlighting the use of the `amt` package for conducting integrated step-selection analyses (iSSA's). You need to install the latest version from CRAN (it was updated on March 6, 2023 in preparation for this workshop!). You will also want to update any dependencies associated with the `amt` package using:

`install.packages("amt", dependencies = TRUE)`

<!---
We will be using several other packages during the workshop. You can install (or update) all of them by running the code in `packages.R`. We strongly recommend that you upgrade to the most up-to-date versions of all these packages.
--->
  
 
## Other Resources

 
**ESA Ecological Forecasting Initiative**: webinar on iSSA by Tal Avgar and Brian Smith. You can find a [recording of the webinar on YouTube](https://youtu.be/jiY9N-TNRjs). You can find the [lecture slides, R code, and Q&A on GitHub](https://github.com/eco4cast/Statistical-Methods-Seminar-Series/tree/main/avgar-smith_issa). You can find the Q&A markdown in the GitHub repo, or [just follow this link](https://github.com/eco4cast/Statistical-Methods-Seminar-Series/blob/main/avgar-smith_issa/Q_and_A.md).

The webinar includes some coded examples of iSSFs that include interactions with the movement parameters that we did not demonstrate in this workshop.
 
