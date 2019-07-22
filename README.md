# distribution-over-quantities

This dataset contains tuples of measurement distributions of nouns, verbs and adjectives.

## Motivation

How much does a lion weigh? How tall can they be? When do people typically eat breakfast? And, how long are concerts?

Most people would know at least an approximate answer to these questions, many of which fall under the notion of commonsense knowledge, and some of which exist in resources such as Wikipedia, or in knowledge graphs like Freebase.

Natural Language Understanding systems should also know, at least approximately, the answers to these questions, to better support questions answering and textual entailment and, more generally, in order to support reasoning about events described in natural language, and converse with people naturally.

We release a resource that characterizes the quantitative distribution of values mentioned in text about properties such as size, duration, weight, etc.  We aggregate the measures and corresponding mentioned values for nouns, adjectives, and verbs.  A detailed explanation of how the dataset was obtained and resuls can be found on the accompanying paper "How Large Are Lions? Inducing Distributions over Quantitative Attributes" published in ACL 2019 (see below for the Bibtex entry).

## Details

THe data has the following format per entry:

['obj', 'head',
'dim', 'mean',
'perc_5', 'perc_25',
'median', 'perc_75',
'perc_95', 'std']
where perc_5 means 5th percentile of measurements

The dimensions are normallzied as follows:

An example:

The resource is hosted in Google Cloud Platform.  Please click on the [link](https://console.cloud.google.com/storage/browser/measures-grounding/) to access the dataset.  The dataset may be freely used for any purpose, although acknowledgement of Google LLC. ("Google") as the data source would be appreciated. The dataset is provided "AS IS" without any warranty, express or implied.  Google disclaims all liability for any damages, direct or indirect, resulting from the use of the dataset. 

## Citation

If you use or discuss this dataset in your work, please cite our paper:

```
@InProceedings{DOQ,
    title = {How Large Are Lions?  Inducing Distributions over Quantitative Attributes},
    author = "Yanai Elazar, Abhijit Mahabal, Deepak Ramachandran, Tania Bedrax-Weiss, Dan Roth},
    booktitle = {Proceedings of ACL 2019},
    year = {2019}
```
