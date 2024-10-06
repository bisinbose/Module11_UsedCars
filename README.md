{\rtf1\ansi\ansicpg1252\cocoartf2709
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fnil\fcharset0 .SFNS-Regular_wdth_opsz180000_GRAD_wght2580000;\f1\fswiss\fcharset0 Helvetica-Bold;\f2\fnil\fcharset0 HelveticaNeue;
\f3\fnil\fcharset0 .SFNS-Regular_wdth_opsz120000_GRAD_wght2580000;\f4\fnil\fcharset0 .SFNS-Regular_wdth_opsz110000_GRAD_wght2580000;\f5\fswiss\fcharset0 Helvetica;
}
{\colortbl;\red255\green255\blue255;\red24\green26\blue30;\red255\green255\blue255;\red0\green0\blue0;
\red0\green0\blue0;}
{\*\expandedcolortbl;;\cssrgb\c12157\c13725\c15686;\cssrgb\c100000\c100000\c100000;\cssrgb\c0\c0\c0;
\cssrgb\c0\c0\c0\c87059;}
\margl1440\margr1440\vieww34360\viewh19080\viewkind0
\deftab720
\pard\pardeftab720\partightenfactor0

\f0\b\fs48 \cf2 \cb3 \expnd0\expndtw0\kerning0
Introduction\
\pard\tx720\tx1440\tx2160\tx2880\tx3600\tx4320\tx5040\tx5760\tx6480\tx7200\tx7920\tx8640\pardeftab720\partightenfactor0

\f1\fs24 \cf0 \cb1 \kerning1\expnd0\expndtw0 	
\f2\b0\fs28 \cb3 \expnd0\expndtw0\kerning0
In this application, used car dataset from kaggle is used. The original dataset contained information on 3 million used cars. The provided dataset contains information\'a0on 426K cars to ensure speed of processing. The goal is to understand what factors make a car more or less expensive. As a result of the analysis, application should provide clear recommendations to the client -- a used car dealership -- as to what consumers value in a used car.
\f1\b \cb1 \kerning1\expnd0\expndtw0 \

\fs24 \
\
\pard\pardeftab720\partightenfactor0

\f3\fs36 \cf2 \cb3 \expnd0\expndtw0\kerning0
The Business Problem\
		
\f2\b0\fs28 Our goal is to determine what particular features of the car are stronger predictors for the price. The data received contains information about the make, model, mechanical differences and specifications, color, and the region it is in. The data also contains the price of the car. Our goal is to fit a model that will select the best features to predict the price of the car.\
		To adequately price a vehicle, we will investigate past transactions and explore the various features impacting a the price at which a vehicle was sold. Using a regression model, we can help make inferences about the optimal price at which a car can be sold.
\f3\b\fs36 \
\
\
Preparing the Data\
		
\f2\b0\fs28 We removed those columns that are not necessary features that could be used to determine the price of the car.  Also rows with missing data is removed.
\f3\b\fs36 \
\
\pard\pardeftab720\partightenfactor0

\f0\fs48 \cf2 Data Analysis\
\pard\pardeftab720\partightenfactor0

\f3\fs36 \cf2 \
		
\f2\b0\fs32 The following features were used to predict the price of the car:\
			
\fs28 \cf5 region\
			price\
			year\
			manufacturer\
			model\
			condition\
			cylinders\
			fuel\
			odometer\
			title_status\
			transmission\
			drive\
			size\
			type
\f3\b\fs36 \cf2 \
\
		
\f2\b0\fs32 For the categorical features, we used label encoding to convert them to numerical values.
\f4\b \
\
		
\f2\b0 I was able to explore various regression models (Linear, Lasso and Ridge). The best model was the Linear Regression model with Polynomial Features of degree 3
\f4\b \

\f3\fs36 \
		
\f2\b0\fs32 Across all models, it was apparent that the features impacting the most the variation of price was the year of the vehicle. 
\f3\b\fs36 \
\
\pard\pardeftab720\partightenfactor0

\f0\fs48 \cf2 Conclusion\
\pard\pardeftab720\partightenfactor0

\f3\fs36 \cf2 		
\f2\b0\fs32 To maximize the price at which a vehicle is sold, dealerships should focus\'a0on the year, fuel, and cylinders
\f3\b\fs36 \
\
\pard\tx720\tx1440\tx2160\tx2880\tx3600\tx4320\tx5040\tx5760\tx6480\tx7200\tx7920\tx8640\pardeftab720\partightenfactor0

\f5\b0\fs24 \cf0 \cb1 \kerning1\expnd0\expndtw0 \
}