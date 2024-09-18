Classify the severity of restaurant health violations with Model Builder

A multiclass classification model using Model Builder to categorize the risk level of restaurant violations found during health inspections.


The data set used to train and evaluate the machine learning model is originally from the San Francisco Department of Public Health Restaurant Safety Scores. For convenience, the dataset has been condensed to include only the columns relevant to training the model and making predictions. You can visit the following website to learn more about the dataset.

Download the Restaurant Safety Scores dataset and unzip it.

Each row in the dataset contains information regarding violations observed during a Health Department inspection and a risk assessment of the threat those violations present to public health and safety.

InspectionType	ViolationDescription	RiskCategory
Routine - Unscheduled	Inadequately cleaned or sanitized food contact surfaces	Moderate Risk
New Ownership	High-risk vermin infestation	High Risk
Routine - Unscheduled	Wiping cloths not clean or properly stored or inadequate sanitizer	Low Risk
InspectionType: the type of inspection. This can either be a first-time inspection for a new establishment, a routine inspection, a complaint inspection, and many other types.
Violation Description: a description of the violation found during the inspection.
RiskCategory: the risk severity a violation poses to public health and safety.
The label is the column you want to predict. When performing a classification task, the goal is to assign a category (text or numerical). In this classification scenario, the severity of the violation is assigned the value of low, moderate, or high risk. Therefore, the RiskCategory is the label. The features are the inputs you give the model to predict the label. In this case, the InspectionType and ViolationDescription are used as features or inputs to predict the RiskCategory.
