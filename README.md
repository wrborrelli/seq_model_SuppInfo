# IBM Rxn for Chemistry Evaluation

This is the supporting information and code for the article _Evaluating the Performance of a
Transformer-based Organic Reaction Prediction
Model_

## Data & Code Information
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
  - t1CMapConfs.txt : RXNMapper map confidences for top-1 correct predictions
  - t1WRmapConfs.txt : RXNMapper map confidences for top-1 incorrect predictions
 */


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

## References
(1) Reactants, products, and transition states of elementary chemical reactions based on
quantum chemistry. Scientific Data 2020, 7, 137.

(2) Schwaller, P.; Laino, T. Machine Learning in Chemistry: Data-Driven Algorithms,
Learning Systems, and Predictions; ACS Symposium Series; American Chemical Soci-
ety, 2019; Vol. 1326; pp 4–61.

(3) Valavanidis, A. Synthetic Organic Chemistry and the Emergence of Artificial
Intelligence-Driven Technology to Synthesize Target Chemical Compounds. 2020, 1,
1–26.

(4) Szymkuć, S.; Gajewska, E. P.; Klucznik, T.; Molga, K.; Dittwald, P.; Startek, M.;
Bajczyk, M.; Grzybowski, B. A. Computer-Assisted Synthetic Planning: The End of
the Beginning. Angewandte Chemie International Edition 2016, 55, 5904–5937.

(5) Segler, M. H. S.; Preuss, M.; Waller, M. P. Planning chemical syntheses with deep
neural networks and symbolic AI. Nature 2018, 555, 604–610.

(6) Coley, C. W.; Rogers, L.; Green, W. H.; Jensen, K. F. Computer-Assisted Retrosyn-
thesis Based on Molecular Similarity. ACS Central Science 2017, 3, 1237–1245.

(7) Schwaller, P.; Vaucher, A. C.; Laino, T.; Reymond, J.-L. Prediction of Chemical Reac-
tion Yields using Deep Learning. 2020; https://chemrxiv.org/articles/preprint/
Prediction{_}of{_}Chemical{_}Reaction{_}Yields{_}using{_}Deep{_}Learning/
12758474https://chemrxiv.org/ndownloader/files/25011413.

(8) Kreutter, D.;Schwaller, P.;Reymond, J.-L. Predicting Enzymatic Reactions
with a Molecular Transformer. 2020; https://chemrxiv.org/articles/preprint/
Predicting{_}Enzymatic{_}Reactions{_}with{_}a{_}Molecular{_}Transformer/
13161359https://chemrxiv.org/ndownloader/files/25313723.

(9) Pesciullesi, G.; Schwaller, P.; Laino, T.; Reymond, J.-L. Transfer learning enables the
molecular transformer to predict regio- and stereoselective reactions on carbohydrates.
Nature Communications 2020, 11, 4874.

(10) Howard, J.; Ruder, S. Universal Language Model Fine-tuning for Text Classification;
2018; pp 328–339.

(11) Devlin, J.; Chang, M.-W.; Lee, K.; Toutanova, K. BERT: Pre-training of Deep Bidi-
rectional Transformers for Language Understanding; 2018.

(12) Schwaller, P.; Laino, T.; Gaudin, T.; Bolgar, P.; Hunter, C. A.; Bekas, C.; Lee, A. A.
Molecular Transformer: A Model for Uncertainty-Calibrated Chemical Reaction Pre-
diction. ACS Central Science 2019, 5, 1572–1583.

(13) Schwaller, P.; Petraglia, R.; Zullo, V.; Nair, V. H.; Haeuselmann, R. A.; Pisoni, R.;
Bekas, C.; Iuliano, A.; Laino, T. Predicting retrosynthetic pathways using transformer-
based models and a hyper-graph exploration strategy. Chemical Science 2020, 11,
3316–3325.

(14) IBM RXN for Chemistry. https://rxn.res.ibm.com.

(15) rxn4chemistry,rxn4Chemistry.2020;https://github.com/rxn4chemistry/
rxn4chemistry.

(16) Borrelli, W. IBMRxnAPI. 2020; https://github.com/wrborrelli/IBMRxnAPI.

(17) Smith, J. G. Organic Chemistry; McGraw-Hill Education, 2017.

(18) Stuart Warren, P. W. Workbook for Organic Synthesis The Disconnection Approach;
John Wiley and Sons, 2009.

(19) Bottcher, T. An Additive Definition of Molecular Complexity. Journal of Chemical
Information and Modeling 2016, 56, 462–470.

(20) Borrelli, W. MolecularComplexityMA. 2020;https://github.com/wrborrelli/
MolecularComplexityMA.

(21) Borrelli, W. Molecular Complexity. 2021; https://resources.wolframcloud.com/
FunctionRepository/resources/MolecularComplexity.

(22) Ertl, P.; Schuffenhauer, A. Estimation of synthetic accessibility score of drug-like
molecules based on molecular complexity and fragment contributions. Journal of Chem-
informatics 2009, 1, 8.

(23) Griffiths,
ralR.-R.;
Sciences:
SynthesisSchwaller,P.;
CaseStudyA
Design.2018;Lee,
inA.Dataset
ChemicalBias
ReactionintheNatu-
Predictionand
https://chemrxiv.org/articles/preprint/
Dataset{_}Bias{_}in{_}the{_}Natural{_}Sciences{_}A{_}Case{_}Study{_}in{_}Chemical{_}
7366973https://chemrxiv.org/ndownloader/files/13616405.

(24) Lowe, D. M. Extraction of Chemical Structures and Reactions from the Literature.
Ph.D. Thesis, University of Cambridge, 2012.

(25) Thakkar, A.; Kogej, T.; Reymond, J.-L.; Engkvist, O.; Bjerrum, E. J. Datasets and
their influence on the development of computer assisted synthesis planning tools in the
pharmaceutical domain. Chemical Science 2020, 11, 154–168.

(26) Schwaller, P.; Hoover, B.; Reymond, J.-L.; Strobelt, H.; Laino, T. Extraction of organic
chemistry grammar from unsupervised learning of chemical reactions. Science Advances
2021, 7, eabe4166.

(27) Jia, X.; Lynch, A.; Huang, Y.; Danielson, M.; Lang’at, I.; Milder, A.; Ruby, A. E.;
Wang, H.; Friedler, S. A.; Norquist, A. J.; Schrier, J. Anthropogenic biases in chemical
reaction data hinder exploratory inorganic synthesis. Nature 2019, 573, 251–255.

## Support
Any questions or correspondences may be directed to wborrelli@fordham.edu.

## Authors and Acknowledgement
Dr. Joshua Schrier, Kim B. and Stephen E. Bepler Chair Professor of Chemistry at Fordham University, was immensely helpful in all aspects of this project. We thank Dr. Bottcher for his inspiration and assistance in developing our code for computing molecular complexity.
