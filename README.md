# Sequence-Based Model Analysis - Supplementary Information 

This is the supporting information and code for the article _Evaluating the Performance of a
Transformer-based Organic Reaction Prediction
Model_

## Data & Code Information
  - transformer_eval_SI.pdf : supporting information document
  - test_set_WB.xlsx : forward synthesis test set
  - test_set_ret_WB.xlsx : retrosynthesis test set
  - combDatAllFwds.csv : all forward synthesis model results 
  - combDatAllRet.csv : all retrosynthesis model results
  - combDatFwds.csv : top-1 forward model results
  - combDatRet.csv : top-1 retrosynthesis model results
  - combFwdDat.csv : top-1 forward results of top-1 retrosynthesis model results
  - figs_and_reacs.nb : Mathematica code for generating figures and reactions
  - retro_analysis.nb : Mathematica code for retrosynthesis analysis
  - synth_analysis.nb : Mathematica code for forward synthesis analysis
  - rmap.ipynb : Python code for RXNMapper analysis
  - t1CMapConfs.txt : RXNMapper map confidences for top-1 correct predictions
  - t1WRmapConfs.txt : RXNMapper map confidences for top-1 incorrect predictions


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
High confidence reactions | Reactions with a confidence above 0.90
Reaction Mapping Results | Results of RXNMapper mappings

## Support
Any questions or correspondences may be directed to wborrelli@fordham.edu.

## Authors and Acknowledgement
Dr. Joshua Schrier, Kim B. and Stephen E. Bepler Chair Professor of Chemistry at Fordham University, was immensely helpful in all aspects of this project. We thank Dr. Bottcher for his inspiration and assistance in developing our code for computing molecular complexity.
