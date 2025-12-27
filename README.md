# linguistic_regression_analysis_scarfs
Predicting successful communication outcomes based on linguistic properties of expressions and relationships between communicators using chi-square tests and linear regression models with fixed effects, random intercepts, and interaction terms

In this project, an analysis of the interactions of certain linguistic properties of the target words and relationships between communicators in a game similar to taboo is presented. Results from the original publication of the SCARFS dataset are recreated as well (Trott et al., 2023). The R Markdown file with the complete analysis can be found at: [regression_analysis_linguistic_data_scarfs.qmd](https://github.com/oishani-b/linguistic_regression_analysis_scarfs/blob/7360c559748635d6f2c0b65d41e33bda42f01bb9/regression_analysis_linguistic_data_scarfs.qmd), and the complete report with detailed analyses, background, and limitations can be found at: [Analyses_Report.pdf](https://github.com/oishani-b/linguistic_regression_analysis_scarfs/blob/7360c559748635d6f2c0b65d41e33bda42f01bb9/Analyses_of_Predicted_Successful_Communication_Based_on_Target_Words_and_Relationship_Types.pdf). Interesting findings from analysis beyond the original publication along with corresponding visualizations are briefly outlined below. A detailed explanation of theoretical background and methods for this analysis can be found in section 4.2 of the [report](https://github.com/oishani-b/linguistic_regression_analysis_scarfs/blob/7360c559748635d6f2c0b65d41e33bda42f01bb9/Analyses_of_Predicted_Successful_Communication_Based_on_Target_Words_and_Relationship_Types.pdf).

The SCARFS dataset consists of nominal referring expressions (NREs) used in a game similar to taboo, where the target word is given to pairs of players who are either strangers or friends, and the possible outcomes are winning, losing by saying a 'taboo' word, and running out of time. 

I observed the interaction effects between Concreteness (a linguistic property of these words determining how concrete or abstract a word is based on human judgements) and the Part of Speech (whether the word is a noun or adjective, specifically) of target words, as well as whether the pair were friends or strangers. I used chi-square tests to evaluate if these variables meaningfully contribute to the prediction of the game outcomes outlined above. 

Findings include:
- A significant effect of an <b>interaction between Concreteness and Part of Speech</b> to model Won vs Lost outcomes, (χ2(1) = 4.60, p < .05), showing a stronger effect of concreteness for nouns than adjectives for these outcomes.
- A significant effect of an <b>interaction between Concreteness and Pair Type</b> (χ2(1) = 6.18, p < .05), showing that higher concreteness helps friends more than it helps strangers.

<img width="1318" height="1234" alt="image" src="https://github.com/user-attachments/assets/17fc396b-3af3-466f-ac2e-2dac5fba5e76" />

Reference Papers and Datasets:

Marc Brysbaert and Boris New. Moving beyond kuˇcera and francis: A critical evaluation of current word frequency norms and the introduction of a new and improved word frequency measure for american english. Behavior Research Methods, 44(4):978–990, 2012.

Marc Brysbaert, Amy Beth Warriner, and Victor Kuperman. Concreteness ratings for 40 thousand generally known english word lemmas. Behavior Research Methods, 46(3):904–911, 2014.

Victor Kuperman, Hans Stadthagen-Gonzalez, and Marc Brysbaert. Age-of-acquisition ratings for 30,000 english words. Behavior Research Methods, 44(4):978–990, 2012.

Jeffrey Pennington, Richard Socher, and Christopher D. Manning. Glove: Global vectors for word representation. In Proceedings of the 2014 Conference on Empirical Methods in Natural Language Processing (EMNLP), pages 1532–1543. ACL, 2014.

Sean Trott, Benjamin Bergen, and Eva Wittenberg. Spontaneous, controlled acts of reference between friends and strangers. Language Resources and Evaluation, 57:1081–1105, 2023. doi: 10.1007/s10579-022-09619-y. URL https://doi.org/10.1007/s10579-022-09619-y.
