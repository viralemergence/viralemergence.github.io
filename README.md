[![Pull updated data](https://github.com/viralemergence/viralemergence.github.io/actions/workflows/jekyll.yml/badge.svg)](https://github.com/viralemergence/viralemergence.github.io/actions/workflows/jekyll.yml)


## Dynamic predictions of betacov-host associations


This is a forward-facing living spreadsheet of predicted host-betacoronavirus associations, based on work from:

> Becker, D., Albery, G. F., Sjodin, A. R., Poisot, T., Dallas, T., Eskew, E. A., ... & Carlson, C. J. (2020). Predicting wildlife hosts of betacoronaviruses for SARS-CoV-2 sampling prioritization. bioRxiv. doi: https://doi.org/10.1101/2020.05.22.111344




Updates to the data can be ensure by submitting the following command:

```

curl -o _data/predictions.csv https://raw.githubusercontent.com/viralemergence/Fresnel/master/BinaryWebsite.csv

```

This serves to update the data from the Fresnel repo and place it in the `_data` folder. 


Then it gets mashed into an html table. 






