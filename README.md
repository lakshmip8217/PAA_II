# This is a Practical Assignment II module 11 exploring regressions on used car prices.

All the updates to the notebook are available in the link https://github.com/lakshmip8217/PAA_II/blob/main/prompt_II.ipynb

The dataset contains 426,000 records, and as part of the preprocessing, we analyzed the data to identify and validate invalid or unrealistic values.
After the the preprocessing and removing the outliers, I applied varioud models to train the data and predict the used car price. With hundred of thousands of observations and polynomial features with dataset size, Polynomial Regression with degree 4 was not able to compute with my system. Since Polymonial Regression with degree 4 was not able to compute, i ended up comparing the degree 2 and 3.

The gain by increasing the degree of the polynomial was marginal in contrast to gains from increasing the regression to a degree 2 and 3. This leads to a less efficent shift on the graph of accuracy vs overfitting.

Although I performed L1 and L2 normalization/regularization. The gain of such approach were negligeable. Across all models, it was apparent that the features impacting the most the variation of price was the year of the vehicle. Afterwards, variation in price were mostly allocated to the odometer, drive, cylinder and fuel.
To maximize the price at which a vehicle is sold, dealerships should focus in order of importance on: 1- Year of the vehicle -- the younger the better 2- The odometer -- the lower the km the better 3- the drive -- higher value when forward or rear wheel 4- Cylinders -- the bigger the engine the more expensive the car 5- Fuel -- gas has higher value 6- transmission -- an automatic transmission will greatly impact the value of the price (notebook has the figure at the end)

By focusing on the 6 attributes to select the vehicles in their inventoy. Dealerships will be able to optimize their inventory. It is important to note that a limitation of this model is the expected profit and inventory turnover. The model does not consider such impacts. Hence, the model would need additional data in this area to offer a proper picture to optimize profits and revenue. For instance, although it is true that the bigger the engine the higher the price. If a dealership only stocks 10 cylinder vehicles, it is unlikely that they will have the clients to sell these vehicles. This may yield in much lower profits and revenue.

