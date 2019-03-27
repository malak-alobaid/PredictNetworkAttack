# PredictNetworkAttack #

This predictive model uses the Canadian Instutite of Cybersecurity dataset, which is organized by day. There are ten days, and for each day a seperate attack scenario was carried out. Each day has normal traffic, and some attacking traffic. All days are merged into one dataframe, then the dataframe is cleaned. Features are engineered, and a model is fitted with Sagemaker.

##### Objective ##### 
determine if a model can tell the difference between benign and malicious traffic (Can we get error less than 50%?). A secondary objective is to learn sagemaker basics and how to train and clean a larger dataset. 

##### Who are the key stakeholders? ##### 
In this case, IT / Security admins would want this tool. This tool could be deployed on the network and trigger alerts for malicious activity, much like a bank sends you a text when their systems detect possibly fraudulent behavior. 

##### What does machine learning offer over the existing solution? ##### 
The existing solution is firewalls and preventative security. This machine learning solution offers glue to catch those who slide through those cracks in the security infrastucure, and shut them down before they do real damage, in real time. 

Because I'm not actually deploying this model on Sagemaker (to save $$$$), I've included only the notebooks here. The CIC applied their own feature extractor to the raw pcap files, which I would like to do in a future project.
* 1. Preprocessing
* 2. Clean
* 3. Feature Engineering
* 4. Model 
* 5. Deploy / package (not done)


The code here is not perfect, shows a 'rough draft' version of working through a problem. I didn't make it perfect because I didn't want to spend more money.. I found a first run through gave a model with 90% accuracy, which was beats the win condition of the model being able to tell benign traffic apart from attacking traffic. Definitely want to explore this more in the future, but this is good enough for now.

##### Next Time #####
Spend more time tuning, check out Sagemakers advanced tuning.
Spend more time feature engineering
Consult network expert / learn more about networks to better feature engineer.
Try some of Sagemakers other algorithms.
