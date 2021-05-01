# EECS738-Project-3---Says-One-Neuron-To-Another-

 Prerequisites:
 Python 3.7
 Numpy
 Pandas

 Introduction:
 In this project, we are going to build a neural network to model the prediction process programmatically for two specific datasets.
	
 Datasets used:

1. Statlog (German Credit Data) Data Set
This dataset classifies people described by a set of attributes as good or bad credit risks. 
	Number of instance: 1000
	Number of attributes : 21 (20 predictive, 1 name)
	Attribute Information:
	Attribute 1: (qualitative) Status of existing checking account A11 	: ... < 0 DM A12 : 0 <= ... < 200 DM A13 : ... >= 200 DM / salary 	assignments for at least 1 year A14 : no  	checking account

	Attribute 2: (numerical) Duration in month

Attribute 3: (qualitative) Credit history A30 : no credits taken/ all credits paid back duly A31 : all credits at this bank paid back duly A32 : existing credits paid back duly till now A33 : delay in paying off in the past A34 : critical account/ other credits existing (not at this bank)

Attribute 4: (qualitative) Purpose A40 : car (new) A41 : car (used) A42 : furniture/equipment A43 : radio/television A44 : domestic appliances A45 : repairs A46 : education A47 : (vacation - does not exist?) A48 : retraining A49 : business A410 : others

Attribute 5: (numerical) Credit amount

Attibute 6: (qualitative) Savings account/bonds A61 : ... < 100 DM A62 : 100 <= ... < 500 DM A63 : 500 <= ... < 1000 DM A64 : .. >= 1000 DM A65 : unknown/ no savings account

Attribute 7: (qualitative) Present employment since A71 : unemployed A72 : ... < 1 year A73 : 1 <= ... < 4 years A74 : 4 <= ... < 7 years A75 : .. >= 7 years

Attribute 8: (numerical) Installment rate in percentage of disposable income

Attribute 9: (qualitative) Personal status and sex A91 : male : divorced/separated A92 : female : divorced/separated/married A93 : male : single A94 : male : married/widowed A95 : female : single

Attribute 10: (qualitative) Other debtors / guarantors A101 : none A102 : co-applicant A103 : guarantor

Attribute 11: (numerical) Present residence since

Attribute 12: (qualitative) Property A121 : real estate A122 : if not A121 : building society savings agreement/ life insurance A123 : if not A121/A122 : car or other, not in attribute 6 A124 : unknown / no property

Attribute 13: (numerical) Age in years

Attribute 14: (qualitative) Other installment plans A141 : bank A142 : stores A143 : none

Attribute 15: (qualitative) Housing A151 : rent A152 : own A153 : for free

Attribute 16: (numerical) Number of existing credits at this bank

Attribute 17: (qualitative) Job A171 : unemployed/ unskilled - non-resident A172 : unskilled - resident A173 : skilled employee / official A174 : management/ self-employed/ highly qualified employee/ officer

Attribute 18: (numerical) Number of people being liable to provide maintenance for

Attribute 19: (qualitative) Telephone A191 : none A192 : yes, registered under the customers name

Attribute 20: (qualitative) foreign worker A201 : yes A202 : no

2. Ionosphere Dataset
Number of instance: 351
Number of attributes : 35 (34 predictive, 1 name)
Dataset Information:
This radar data was collected by a system in Goose Bay, Labrador. This system consists of a phased array of 16 high-frequency antennas with a total transmitted power on the order of 6.4 kilowatts. The targets were free electrons in the ionosphere. "Good" radar returns are those showing evidence of some type of structure in the ionosphere. "Bad" returns are those that do not; their signals pass through the ionosphere.
Received signals were processed using an autocorrelation function whose arguments are the time of a pulse and the pulse number. There were 17 pulse numbers for the Goose Bay system. Instances in this databse are described by 2 attributes per pulse number, corresponding to the complex values returned by the function resulting from the complex electromagnetic signal.
Attribute Information:¶
-- All 34 are continuous -- The 35th attribute is either "good" or "bad" according to the definition summarized above. This is a binary classification task.


Idea: A neural network is defined as a computational system which has a number of highly interconnected simple elements/nodes, called ‘neurons’. These neurons are organized in layers which process information using dynamic responses of each state to external inputs. Neural network can be used to classify the good or bad electron structure class for ionosphere dataset and people’s good or bad credit risks for the German credit data dataset. Neural network can be used to group the unlabeled data and according to similarities between the attributes of the samples and can predict the class of the samples.

Detailed steps:
Implementation steps are explained in the Neural Network-ionosphere.ipynb and Neural Network-German Credit Card.ipynb files for the respective datasets. All the steps of implementations of neural network are discussed along with the functionalities in those files.

 Result:
* Iterations: We can see that Neural network has taken 100 iterations for the Ionosphere dataset and 10 iterations for the German Credit dataset to converge.
* Accuracy: We have got a testing accuracy of 77.3% for the Ionosphere dataset and 62.6% for the German Credit card dataset. We have also observed a training accuracy of 94.4% for the Ionosphere dataset and 71.5% for the German Credit card dataset. 
* Sample test: We have also tested a sample after training for both the dataset and the model has predicted correct class for the tested sample for both.

 Built With:
 Python 3.7
 Jupyter Notebook

 Authors:
 Ashwin Rathore

 License:
 This project is created for Course EECS 738 Assignment for University of Kansas.

 Acknowledgments:
 https://archive.ics.uci.edu/ml/datasets/statlog+(german+credit+data)
 https://archive.ics.uci.edu/ml/datasets/ionosphere 

