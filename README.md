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

## Model 4
Adjusted the inputs. This model produced similar accuracy, but the precision and recall were much better. While still not acceptable (below 0.9), they are getting better.

## Model 5
Added input for the Kepler Band. The accuracy decreased slightly.

# Conclusion
I believe my 4th model is the best model. This model takes information about the plant (temperature, radius, transit time) and its orbiting star (size, temp, etc) and uses it to predict potential Kepler objects of interest. This makes sense as these inputs would determine the potential to sustain life for any kepler object. This model also had the best precision/recall while obtaining the greatest accuracy. It could be modified to include more inputs, but I found them to add very little value while further complicating the model. This model has been labeled "best fit" in the main folder.
