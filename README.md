# Background

Sterile filtration is a vital step in manufacturing of drugs that are administered e.g. intraveneous. A high bioburden level prior to the sterile filtration step increases the risk of compromizing the sterile filter. Accordingly, reducing bioburden prior to final sterile filtration is crucial for effective microbial control and risk mitigation in drug manufacturing.

The European Medicines Agency (EMA) guidelines [EMA/CHMP/CVMP/QWP/850374/2015](https://www.ema.europa.eu/en/documents/scientific-guideline/guideline-sterilisation-medicinal-product-active-substance-excipient-primary-container_en.pdf) stae that the maximum acceptable bioburden before filtration must be specified in the application, typically not more than 10 colony-forming units (CFU) per 100 ml, depending on the volume to be filtered and the filter diameter. 
If the bioburden exceeds this, pre-filtration through a bacteria-retaining filter is required. The EMA guidelines also allow for a smaller pre-/filtration volume to be tested if justified due to limited availability of the medicinal product in the early stage of drug development.

Ideally, multiple samples are taken from each batch and tested for microbial counts. However, 100 mL of drug substance or drug product is not a small amount, especially for high value products. Smaller samples (e.g. 10 mL) would be preferable. Due to the variability and limited sensitivity of microbiological analyses, for small sample size the measured microbial count may be inaccurate. This variability may lead to either rejecting a batch with an actual bioburden level below the limit or accepting a batch with a bioburden level above the limit. 

As [Yang et al.](https://journal.pda.org/content/67/6/601) point out in their paper "A Risk-based Approach to Setting Sterile Filtration Bioburden Limits", modeling shows a 33.4% chance to reject a batch with a true bioburden level of 9 CFU/100 mL and a 50% chance to accept one with 11 CFU/100 mL. 

This repo explores their approach in Python and provides a method to calculate bioburden limits based on the proposed risk based approach and experimental data.

# Files

- The notebook [yang_2013](yang_2013.ipynb) does reproduce the figures from the publication of Yang e. al. in Python.
- The notebook [dist_fit_mle](dist_fit_mle.ipynb) does explore maximum likelihood for calculating bioburden limits incorporating assay variability.

# Status

Currently I am working on the documentation as well as clarity of the results.

# Literature

[Yang et al.](https://journal.pda.org/content/67/6/601)

[Statistics for Biotechnology Process Development](https://www.taylorfrancis.com/books/edit/10.1201/9781315120034/statistics-biotechnology-process-development-todd-coffey-harry-yang)

[Bayesian Methods in Pharmaceutical Research](https://www.taylorfrancis.com/books/edit/10.1201/9781315180212/bayesian-methods-pharmaceutical-research-emmanuel-lesaffre-gianluca-baio-bruno-boulanger)
