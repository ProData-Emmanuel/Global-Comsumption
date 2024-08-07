### This text file explains the projects contained in the two Notebooks included in this folder:

1. Time Series Analysis to understand Electricity consumption per household. A type of Artificial Neural Network called LSTM (see the notebook)

2. Binary Classification Task to predict whether electric grids are stable or not.


PROJECT 1
TITLE: Regression/Clustering: Time Series Analysis
OBJECTIVE: Apply Time Series Analysis-- Regression / Clustering, to Predict Household Electric Power Consumption.
	   To understand Electricity consumption per household using Long Short-Term Memory (LSTM).
METHOD:
-predict the active power consumption for the next N minutes given the consumption for the p former minutes. p is a hyper parameter of the model ( window width ).
-Make Predictions usind Traditional Machine learning algorithms, AR, ARIMA, SARIMAX
-Evaluate the models and compare results from the AR, ARIMA & SARIMA mthods with predictions from the Recurrent Neural Network, RNN.
Conclude by visualizing the compared models.

Data Source: https://archive.ics.uci.edu/ml/datasets/individual+household+electric+power+consumption




=============================================================================================================

### PROJECT 2
#### TITLE: Electricity Grid System Stability
#### OBJECTIVE: To Predict whether electric grids are stable or not.

DESCRIPTION/METHOD:
Electrical grids require a balance between electricity supply and demand in order to be stable. Conventional systems achieve this balance through demand-driven electricity production. For future grids with a high share of inflexible (i.e., renewable) energy source, the concept of demand response is a promising solution. This implies changes in electricity consumption in relation to electricity price changes. In this work, different algorithms were used to built binary classifiers to predict if a grid is stable or unstable using the UCI Electrical Grid Stability Simulated dataset. Performnce Metrics are used to determine the accuracy of the predictions.

**Dataset Source:** https://archive.ics.uci.edu/ml/datasets/Electrical+Grid+Stability+Simulated+Data+
It has 12 primary predictive features and two dependent variables.

#### Predictive features:	
1.	'tau1' to 'tau4': the reaction time of each network participant, a real value within the range 0.5 to 10 ('tau1' corresponds to the supplier node, 'tau2' to 'tau4' to the consumer nodes);
2.	'p1' to 'p4': nominal power produced (positive) or consumed (negative) by each network participant, a real value within the range -2.0 to -0.5 for consumers ('p2' to 'p4'). As the total power consumed equals the total power generated, p1 (supplier node) = - (p2 + p3 + p4);
3.	'g1' to 'g4': price elasticity coefficient for each network participant, a real value within the range 0.05 to 1.00 ('g1' corresponds to the supplier node, 'g2' to 'g4' to the consumer nodes; 'g' stands for 'gamma');

#### Dependent variables:
1.	'stab': the maximum real part of the characteristic differential equation root (if positive, the system is linearly unstable; if negative, linearly stable);
2.	'stabf': a categorical (binary) label ('stable' or 'unstable').