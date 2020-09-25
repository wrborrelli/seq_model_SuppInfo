# IBM Rxn for Chemistry Evaluation

This is an evaluation of the IBM Rxn for Chemistry molecular transformer architecture as applied to retrosynthetic prediction. 

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
(1) Schwaller, P.; Petraglia, R.; Zullo, V.; Nair, V. H.; Haeuselmann, R. A.; Pisoni, R.;
Bekas, C.; Iuliano, A.; Laino, T. Predicting retrosynthetic pathways using transformerbased models and a hyper-graph exploration strategy. Chemical Science 2020, 11, 3316{
3325.
(2) Schwaller, P.; Laino, T.; Gaudin, T.; Bolgar, P.; Hunter, C. A.; Bekas, C.; Lee, A. A.
Molecular Transformer: A Model for Uncertainty-Calibrated Chemical Reaction Prediction. ACS Central Science 2019, 5, 1572{1583.
(3) IBM RXN for Chemistry. https://rxn.res.ibm.com.
(4) rxn4chemistry, rxn4Chemistry. 2020; https://github.com/rxn4chemistry/
rxn4chemistry.
(5) Borrelli, W. IBMRxnAPI. 2020; https://github.com/wrborrelli/IBMRxnAPI.
(6) Smith, J. G. Organic Chemistry; McGraw-Hill Education, 2017.
9(7) Bottcher, T. An Additive Definition of Molecular Complexity. Journal of Chemical Information and Modeling 2016, 56, 462{470.
(8) Borrelli, W. MolecularComplexityMA. 2020; https://github.com/wrborrelli/
MolecularComplexityMA.
(9) Ertl, P.; Schuffenhauer, A. Estimation of synthetic accessibility score of drug-like
molecules based on molecular complexity and fragment contributions. Journal of Cheminformatics 2009, 1, 8.

## Support
Any questions or correspondences may be directed to wborrelli@fordham.edu.

## Authors and Acknowledgement
Dr. Joshua Schrier, Kim B. and Stephen E. Bepler Chair Professor of Chemistry at Fordham University, was immensely helpful in all aspects of this project. 
