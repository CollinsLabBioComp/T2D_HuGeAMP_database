# T2D HuGeAMP database
`T2D_HuGeAMP_data.tsv`: Data from [Human Genetics Knowledge Portal's type II diabetes (T2D) dataset](https://md.hugeamp.org/method.html?trait=t2d&dataset=mccarthy) formatted into a .tsv file for offline usage.

From their website:
>The curated T2D effector gene predictions from Anubha Mahajan and Mark McCarthy synthesize multiple kinds of biological evidence to classify the potential of genes to be causal for T2D.

## About the data
The formatted data contains the following columns:
* `gene` : HGNC symbol (ex: `INS` for insulin)
* `initial_alias` : symbol fed into https://biit.cs.ut.ee/gprofiler/convert for automatic conversion to Ensembl IDs
* `alias_concordance` : TRUE if the values for `gene` and `initial_alias` are identical. 
  *  Two (2) genes had synonyms and were mapped as follows: `FAM63A`	-> `MINDY1` and `PTRF`	-> `CAVIN1`
* `ensembl_id` : the Ensembl ID corresponding to `initial_alias` 

For `combined_prediction`, `combined_genetic_evidence`, `combined_regulatory_evidence`, and `combined_perturbation_evidence`, please refer to the [original documentation](http://3.208.176.209/sites/default/files/documents/effector_predictions_documentation.pdf).


## Original data
To reference the webpage this was scraped from, see the cached .html file which was saved using [SingleFile](https://github.com/gildas-lormeau/SingleFile). This webpage was last scraped and cached on: `(12_13_2021 2_50_27 PM)`

Please reach out or submit a pull request if there is an issue with the data!


Data scraped and formatted by [Caleb Grenko](mailto:cal.grenko@nih.gov).  

`T2D_kp_effector_genes.txt`: Data from [Human Genetics Knowledge Portal's type II diabetes (T2D) dataset](https://t2d.hugeamp.org/method.html?trait=t2d&dataset=egls) formatted into a .txt file for use. Note, this is a list different from the above one. The list was compiled from the web site by Narisu. 

From their website:
>The T2D Effector Prediction Summary integrates the results of the three methods shown on the Effector gene predictions page for prediction of type 2 diabetes effectors: the Curated T2D effector gene predictions, the Effector index predictions (EIP in the table below), and the Integrated Classifier predictions (ICP in the table below). Note that the top genes predicted by the curated approach may have been used as positive controls or training sets for the other two methods and thus may not appear in those results.


### Disclaimer
This is <ins>not</ins> an official repository for HuGeAMP. It is not endorsed by the original publishers, and the user accepts all responsibility for verifying the accuracy and integrity of the data. 
