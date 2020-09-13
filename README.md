# 
This is a repository made in a purpose of final project for Data Science Bootcamp

Business case: Once upon a time there was a leasing company. To keep its position on market it has to have good and comprehensive offer for customers but at the same time continiusly improve processes. Having fast credit decision process makes us more prone to be chosen by customers. Company implemented automatic desision process several years ago, starting with most standaraised products (leasing for a new car) and currently having several different product and customer types covered. But there is still place for improvement. Generaly transaction can be approved automaticaly if at least several condistions are fulfield: credit scoring is acceptable, policy criteria are met, there is not fraud warrings and customer has more or less "standard" profile. If transaction is not approved automaticaly, then there are 2 possible paths: rejection or going for manual analysis. This project is focused on investigate these transacions which went through manual analysis. If there is a space of further improvement of automatisation. If model is able to predict with good accuracy if credit analyst is going to accept transaction - these predictions can be used to get several more applications into automatic process (because with high probablity analys would either way accept it).

So starting point is to have all transactions, which went threw 'non automatic' process (around 20 tsd cases), for them we have information if they were manualy accepted ('ManAkc' column). Data set is closed to balanced because there was 67% of manualy accepted transactions, so there is no need for resampling data. Number of explanatory variables is very high, but some of them are correlated (they are transformation of themselves).

Problem to solve is binary classifiaction, data came from sql database (I prepared them on SQL, so only result of data manipulation is imported to python).

Some technical remarks:
a) I had to change some strings into '#$#$%#$^#' for example data base connection (because they were expicit)
b) I had to delete every personal or sensitive informations
c) Due to data specifity I had to work on my company's laptop which is super slow, that is why I didn't tested many possible combinations in grid search

