# IBM Rxn for Chemistry Evaluation

This is an evaluation of IBM Rxn for Chemistry molecular transformer architecture as applied to retrosynthetic prediction. 

The Mathematica notebook named "ibmRxnRetro.nb" is the raw notebook used for analysis while the "ibmRxnRetro_Formatted.nb" is slightly abbreviated, more neatly formatted, and includes annotation for my reasoning for my code. 

A formal write-up of my analysis and results is available in the "wb_ibmRxnEval.pdf". A condensed results section is what follows.

## Results 
The following table summarizes the analyses done and results, where applicable:
Analysis | Visualization
------- | ------ |
ΔSA (synthetic accessibility) | Scatter plots and histogram distributions 
ΔCm (molecular complexity) | Scatter plots and histogram distributions
Confidence Distributions | Histogram distributions and box and whisker plots
Non-canonical vs. canonical Input SMILES | Reactions that produced different products for non-canonical vs. canonical input SMILES
Sameness of Retrosynthetic and Forward Predictions | Reactions that did not produce the product that the literature source claims it should produce
Reactions with ΔSA > 0 | Reactions that saw an increase in synthetic accessibility going from reactants to products
Reactions with ΔCm > 0 | Reactions that saw an increase in molecular complexity going from reactants to products
Low confidence reactions | Reactions with a confidence below 0.1 
Round Trip Analysis | Percentage of suggested retrosyntheses of a unique reaction class that forms the same product
Coverage Analysis | Percentage of times at least one correct retrosynthetic sequence is given 
ISMI % | Percentage of proposed SMILES that are invalid 

## References
(1) Ertl, P.; Schuffenhauer, A. Estimation of Synthetic Accessibility Score of Drug-like Molecules Based on Molecular Complexity and Fragment Contributions. J. Cheminform. 2009, 1 (1), 8. https://doi.org/10.1186/1758-2946-1-8.

(2) Schwaller, P.; Petraglia, R.; Zullo, V.; Nair, V. H.; Haeuselmann, R. A.; Pisoni, R.; Bekas, C.; Iuliano, A.; Laino, T. Predicting Retrosynthetic Pathways Using Transformer-Based Models and a Hyper-Graph Exploration Strategy. Chem. Sci. 2020, 11 (12), 3316–3325. https://doi.org/10.1039/C9SC05704H.

(3) Schwaller, P.; Laino, T.; Gaudin, T.; Bolgar, P.; Hunter, C. A.; Bekas, C.; Lee, A. A. Molecular Transformer: A Model for Uncertainty-Calibrated Chemical Reaction Prediction. ACS Cent. Sci. 2019, 5 (9), 1572–1583. https://doi.org/10.1021/acscentsci.9b00576.

(4) Böttcher, T. An Additive Definition of Molecular Complexity. J. Chem. Inf. Model. 2016, 56 (3), 462–470. https://doi.org/10.1021/acs.jcim.5b00723.

## Support
Any questions or correspondences may be directed to wborrelli@fordham.edu.

## Authors and Acknowledgement
Dr. Joshua Schrier, Kim B. and Stephen E. Bepler Chair Professor of Chemistry at Fordham University, was immensely helpful in all aspects of this project. 
