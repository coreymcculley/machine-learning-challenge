# machine-learning-challenge
Bootcamp HW for Machine Learning


## Pre Processing
Before working on the assigned dataset, I read through the explanation of the column headers on the KOI webpage provided. This allowed me to understand more about the possible importance of each variable to my model. 

## Model 1
Based on what I was able to learn from the KOI definitions, I thought a good initial model would take into account the "boolean" variables pertaining to the orbits of the KOI (first 4 columns of the spreadsheet). Using these variables, I was able to obtain a model with an accuracy near 50%, so my understanding of the variables appears to be somewhat reasonable. I will begin adding additional information to try and get better results for my model. 

## Model 2
Added the orbital transit time, impact (distance from stellar object), planet radius (koi_prad),  planet temp (koi_teq), and star temp (koi_steff). Model accuracy increased slightly, but by looking at the random forest importance scores, I see that that first 4 variables have low importance. They will be removed and I will look for additional info in next model.

## Model 3
Adding more of the star properties while removing the initial model variables. Accuracy decreased slightly but was still around 50%.