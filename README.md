# King Count Housing Data Project

## Business Goal

To provide an accurate estimate of a homes sell values within a reasonable margin of error as well as insight and advice on what a home owner can do to their home to make it more attractive on the market as well as increasing value of said home.

## The Data

This project uses the King County House Sales dataset, which can be found in  `kc_house_data.csv` in the data folder in this repo. The description of the column names can be found in `column_names.md` in the same folder. 

## Baseline Model

This model was meant to serve as a baseline model to assess the quality of the data set as is.

Columns 'id', 'date', 'view', 'zipcode', 'lat', 'long', 'sqft_living15', and 'sqft_lot15' were removed to prevent noise in data.

* Model returned Aprox. 64% explainable variance in predictions
* Model returned Aprox. $220,000 margin of error in home value prediction.

## Model 2

Model was made to remove outliers in data for a more accurate prediction as well as return a smaller margin of error on home value prediction.

* Model returned decrease in accuracy at Aprox. 60% explainable variance.
* Model returned decrease in margin of error in home value prediction to Aprox. $169,669.

## Model 3

Model was made as a test to see how much of the initially removed data affects the model.

Columns 'id', 'date' remain removed to prevent noise in data.

columns 'view', 'zipcode', 'lat', 'long', 'sqft_living15', and 'sqft_lot15' were added back into the model.

* Model returned increase in accuracy at Aprox. 69% explainable variance.
* Model returned increase in margin of error in home value prediction to Aprox. $202,821.

## Final Model

Final model served as a combination of Models 2 and 3 to create a more accurate model.

* Model returned increase in accuracy at Aprox. 69% explainable variance.
* Model returned decrease in margin of error in home value prediction to Aprox. $117,124.

## Results

Model is able to provide reasonable insight into improvements to a home to make it more valueable and provides a home values within a $117,124 margin of error.