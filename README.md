**Introduction**
	  		
 In this application, used car dataset from kaggle is used. The original dataset contained information on 3 million used cars. 
     The provided dataset contains information on 426K cars to ensure speed of processing. 
     The goal is to understand what factors make a car more or less expensive. 
     As a result of the analysis, application should provide clear recommendations to the client -- a used car dealership -- as to what consumers value in a used car.

**The Business Problem**	
			
   Our goal is to determine what particular features of the car are stronger predictors for the price. 
   The data received contains information about the make, model, mechanical differences and specifications, color, and the region it is in. 
   The data also contains the price of the car. Our goal is to fit a model that will select the best features to predict the price of the car.
			
   To adequately price a vehicle, we will investigate past transactions and explore the various features impacting a the price at which a vehicle was sold. Using a regression model, 
   we can help make inferences about the optimal price at which a car can be sold.


**Preparing the Data**  
			
   We removed those unnecessary features that could be used to determine the price of the car.  Also rows with missing data is removed.

**Data Analysis**
		  
    The following features were used to predict the price of the car:
			region
			price
			year
			manufacturer
			model
			condition
			cylinders
			fuel
			odometer
			title_status
			transmission
			drive
			size
			type
  For the categorical features, we used label encoding to convert them to numerical values. 
   I was able to explore various regression models (Linear, Lasso and Ridge). The best model was the Linear Regression model with Polynomial Features of degree 3.
   Across all models, it was apparent that the features impacting the most the variation of price was the year of the vehicle.

		

**Conclusion**   
		
  To maximize the price at which a vehicle is sold, dealerships should focus on the year, fuel, and cylinders
