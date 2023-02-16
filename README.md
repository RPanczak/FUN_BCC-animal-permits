
## Animal permits in Brisbane as indicators of socioeconomic position.

[Website](https://rpanczak.github.io/FUN_BCC-animals/) with more details.  

### Dog cost

Distribution of dogs across breeds with indication of 'expensive' ones:  

![image](https://user-images.githubusercontent.com/31648642/168630145-12ab079b-91d5-46f7-a3cc-ab7e49df2c47.png)

Spatial distribution of dogs across neighbourhoods, with proportion of expensive ones:  

![image](https://user-images.githubusercontent.com/31648642/168630836-5d914f23-abb9-43de-b8c3-0f14d27c1f20.png)

### Dog breeds used to predict deprivation

Best model to predict *Index of Education and Occupation* turned out to be **XGBoost**. Here is the prediction from the best tuned model:  

![image](https://github.com/RPanczak/FUN_BCC-animal-permits/blob/master/results/pred.png)  

Following breeds were found to be most important in predicting the outcome:  

![image](https://github.com/RPanczak/FUN_BCC-animal-permits/blob/master/results/vim.png)   

More details on the comparison of the models can be found [here](https://rpanczak.github.io/FUN_BCC-animal-permits/13_DALEX.html) and full XGBoost analyses are [here](https://rpanczak.github.io/FUN_BCC-animal-permits/09_xgb.html).  

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
