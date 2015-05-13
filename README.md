# model-comparison-r-julia
Comparison of statistical models from experimental data in R and Julia

## Comparing statistical models in R and Julia
When evaluating experimental data, implementing the statistical analyses in R is generally seen as the best way to go. Though other packages are available (SAS, JMP, SPSS, Stata, Python, etc.) R is open-source and used by a wide community of statisticians and others who need to use its power for statistical analysis. One issue that may arise when dealing with reproducible research is how you know if the models that were fit make sense and the results are consistent across environment. This is important, as not all statistical analysis packages are adept at fitting complex models, especially Linear Mixed Models (LMMs). In order to check the modeling performed, especially for complex calls, I recently decided to re-implement my analyses in other languages (e.g., the Python modules `Statsmodels` and `scikit-learn` when possible) but more often, using the Julia programming language.  

Julia is a good alternative as it can implement not only simple linear models and Generalzed Linear Models (GLMs) but also mixed models via the `MixedModels` package. For LMMs especially, this is a good way to check especially for complicated model calls.  

I analyze three different datasets:  
- published data from an audiovisual perception study  
- published data from a magnetoencephalography (MEG) study  
- psychophysical data from an AX study from my dissertation (not yet published)  

The analyses are contained in two IPython-based notebooks. The first implements the analyses in R using the IPython engine. The second implements the analyses in Julia using the Julia engine. The analyses largely agree between the two comparisons. The notebooks serve as a good learning tool for model calls, evaluation and QA.
