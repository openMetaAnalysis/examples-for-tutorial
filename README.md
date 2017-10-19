# Creating your first meta-analysis

Example meta-analysis:
* https://openmetaanalysis.github.io/tramadol

Background reference on interpreting meta-analyses:
* Cornell JE, Liao JM, Stack CB, Mulrow CD. Annals Understanding Clinical Research: Evaluating the Meaning of a Summary Estimate in a Meta-analysis. Ann Intern Med. 2017 Aug 15;167(4):275-277. doi: [10.7326/M17-1454](https://doi.org/10.7326/M17-1454). PMID: [28785763](https://pubmed.gov/28785763) _Ask me for an annotated PDF of this article._

## Monday (day 1)
* Use the file I sent you ([example format](data/all-studies.csv)) that underlies the clinical outcome you selected in your Cochrane review, upload the file to [openMetaAnalysis editor](https://openmetaanalysis.ocpu.io/home/www/editor.html). Select the measure type (usually relative risk). Do you get the same numbers as Cochrane? Change the Hartung-Knapp setting if needed.
* Search the individual studies at [PubMed](https://pubmed.gov) and add the PMIDs to the csv file. Add to the data file whether each trial was registered (search for 'regis' in the abstracts and articles). These will be needed for your update searches on Wednesday

## Tuesday (day 2)
Assessing non-clinical biases in studies:
* Do a subgroup analysis:
  * Registered vs non-registered trials ([example](https://github.com/openMetaAnalysis/back-pain-chronic-treatment-with-tramadol/blob/master/files/forest-plots/Outcome-Primary.png))
* Make meta-regressions ([examples](https://github.com/openMetaAnalysis/Early-goal-directed-therapy-for-septic-shock/blob/master/files/metaregression/All%20factors.png)).
  * Study size vs effect size.
  * Control rate of events vs effect size 
  * Year of publication vs effect size.

Did any of these yield significant p-values and reduce heterogeneity?

Assessing for clinical biases in studies
* Can you think of a clinical explanation for heterogeneity in the study results? If so, determine which studies have this reason and indicate it in a column for cofactors as done in the [CSV file](https://github.com/openMetaAnalysis/back-pain-chronic-treatment-with-tramadol/tree/master/files/data) for the example meta-analysis above.

## Wednesday (day 3)
Updating the Cochrane meta-analysis. While you probably do not have time to find all relevant studies for a full update, try to at least add 1-2 studies to the Cochrane review.
* Find an alternative meta-analysis on the same topic. Make a table that reconciles the trials included in the two meta-analyses ([example for the tramadol meta-analysis](https://github.com/openMetaAnalysis/back-pain-chronic-treatment-with-tramadol/tree/master/files/reconciliation-tables)) Does this lead you to add or drop any studies from the Cochrane review? If so, does the revised meta-analysis have important changes in results?
* Find newer studies with search methods that do not require search terms:
  * PubMed vector space model (relevancy, algebraic, partial match, ranking) ([example for tramadol meta-analysis](https://github.com/openMetaAnalysis/back-pain-chronic-treatment-with-tramadol/blob/master/files/searching/evidence-search.md))
  * Google Scholar cited reference search ([example for tramadol meta-analysis](https://github.com/openMetaAnalysis/back-pain-chronic-treatment-with-tramadol/blob/master/files/searching/evidence-search.md))
