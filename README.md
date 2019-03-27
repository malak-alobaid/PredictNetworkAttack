# PredictNetworkAttack

This predictive model uses the Canadian Instutite of Cybersecurity dataset, which is organized by day. There are ten days, and for each day a seperate attack scenario was carried out. Each day has normal traffic, and some attacking traffic. All days are merged into one dataframe, then the dataframe is cleaned. Features are engineered, and a model is fitted with Sagemaker.

Because I'm not actually deploying this model on Sagemaker (to save $$$$), I've included only the notebooks here. The CIC applied their own feature extractor to the raw pcap files, which I would like to do in a future project.
* 1. Preprocessing
* 2. Clean
* 3. Feature Engineering
* 4. Model 
* 5. Deploy / package (not done)
