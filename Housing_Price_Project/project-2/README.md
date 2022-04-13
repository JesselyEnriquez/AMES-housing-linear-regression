---


# Iowa Real Estate Investment Study

---
## Problem Statement
Iowa Real Estate Investors Association (IaREIA) based in Des Moines, Iowa looking to potentially begin investments in Ames, Iowa and has reached out to get a strong predictive model, ready to base their investment plans.

## Background
<br>
The Ames Housing Dataset that is avaliable through Kaggle will be utilized for this initial study, throughout this project we will identify what features of a home are the best predictors and evaluate our model based on our R2 scores and RMSE, with a few addition error metrcis. A selection of a couple models will then be uploaded to Kaggle for scoring on brand new data to evaluate the performance (the best will be the final model).

<br>

This is particularly created to assit IaREIA but can be easily utilized for homeowner to help guide their
This is to inform students that plan to apply in their own state If they should expect their scores to be advantages for public schools, however, being in-state applicant should give them a leg up on out-of-state applicants.

---

## Outside Research

Initially before undertaking any data cleaning or analysis, basic background research was undertaken to gain high level insight of what could potentially be features of interest when moving forward. The [hedonic pricing method](https://corporatefinanceinstitute.com/resources/knowledge/valuation/hedonic-pricing/) was the clearest and intuitive concept to utilize. This method is typically used in the economics domain to value, in our case, houses based on the features of a house, in this case the following features were selected intially to group  location and property features. Typically environmental features are included but will not be since data is not avaliable in our particular dataset.


| Original Characteristic |
| --- |
| Property Size     |
|Location Desireability    |
|Amenities Proximity  |
|Number of Rooms  |
| Number of baths  |
|Age  |
|Condition of the house  |
|Construction Materials  |


-----


## Conclusion and Recommendations

Unfortunately, from this model  cannot determine that there is any statistical significance between the features and salesprice.
Based on the results of the study the recommendations below to inform future property invesments of what house traits to pay attention when moving forward on Ames, Iowa investments. These conclusions were based on the more feaures with greater absolute value of the final multiple linear regression model (shown below). Additionally this model could be very useful for homeowners that are in the stage of selling their house, it could be utilized as a tool to set  an accurate sale price or inform them of where they want to focus their remoding efforts in.

Recommendations:
- Location Desirability - houses in houses IN Green Hills, Stone Brook, Northridge,  Northridge Heights avoiding Edwards in particular
- Construction Materials - houses with Wood Shingles rather than Clay or Tile for roof material
- Condition of the house - houses with Excellent exterior quality and kitchen quality, as well as houses with good garage quality
- Amenities Proximity    - houses with  average proximity to various (conditions)
- Avoid investing in houses with Brick Face exteriors

## Future Steps

More exploration can be conducted tot determine if more tinkering with the final model could create a stronger predicitive model than produced here. Additionally a deeper consideration could be undertaken for the ordinal vs discrete features potentially translating them as categorical to see if the models perfomance would change.
