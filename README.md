
**Comparative Study of different Feature Extraction Techniques**
* Cancer Gene Expression Data:
	* [Leukemia](https://file.biolab.si/biolab/supp/bi-cancer/projections/info/leukemia.html)
	* [DLBCL](https://file.biolab.si/biolab/supp/bi-cancer/projections/info/DLBCL.html)
	* [Lung](https://file.biolab.si/biolab/supp/bi-cancer/projections/info/lung.html)

* Machine Learning Feature Extraction Task:

	* The study of gene expression of cells and tissue is one of the major ways for discovery in
		medicines. The main challenge of such gene data is high input dimensionality, heterogeneity in
		the data with very low sample size. To overcome this, gene subset selection/Feature Selection
		has become a crucial and essential step.
	* **A.** Applied the three filter methods(1. **Mutual Info[f1]** 2. **F Classif[f2]** and 3.**T-Test[f3]** ) on
		the three datasets to get important features( N: No. of selected feature is not restricted butit should be less than 20% of toat features). Used KNN(C1) and SVM(C2) for
		Classification. Report Accuray, F-Score, and Confusion Matrix.
	* **B.** Selected the most important N/3 features from each of these three filter methods(f1,f2,f3).<br> $F =  f_1\cupf_2\cupf_3$
		<br>Classified the test data with the Classifiers(C1 and C2) and Compared them with the above
		result.
	* **C.** Now applied feature selection in a cascaded manner and Classify with C1 and C2.
			* a. F1( N features ) → F2( 2N/3 features out of selected features from F1) → F3(N/3
				 features out of selected features from F2)
			* b. F2 → F3 → F1
			* c. F3 → F1 → F2
	* **D** Classify the test data using wrapper methods(Sequential Forward Search and Sequential
			Backward Search ) with N features.

**Output Inferences**<br>
The output inference for each dataset can be found in their respective folders

