For this part of the assignment, you’ll write a report on the performance of the deep learning model you created for Alphabet Soup.

The report should contain the following:

    Overview of the analysis: Explain the purpose of this analysis.

    Results: Using bulleted lists and images to support your answers, address the following questions:

    Data Preprocessing
        What variable(s) are the target(s) for your model?
        app_dummies_df['IS_SUCCESSFUL'] 
        Binary result of funded ventures
        
        What variable(s) are the features for your model?
        app_dummies_df.drop(columns='IS_SUCCESSFUL')
        AFFILIATION—Affiliated sector of industry
        CLASSIFICATION—Government organization classification
        USE_CASE—Use case for funding
        ORGANIZATION—Organization type
        STATUS—Active status
        INCOME_AMT—Income classification
        SPECIAL_CONSIDERATIONS—Special considerations for application
        ASK_AMT—Funding amount requested
        
        What variable(s) should be removed from the input data because they are neither targets nor features?
        EIN and NAME—Identification columns
        APPLICATION_TYPE—Alphabet Soup application type

    Compiling, Training, and Evaluating the Model
        How many neurons, layers, and activation functions did you select for your neural network model, and why?
        I experimented with different quantities of neurons, layers, and activation functions to hopefully increase model performance. I added more nodes, layers, and 
        epochs incrementally based on previous iterations. 
        The optimized version of my model has 100 nodes in layer 1, 40 in layer 2, and 20 in layer 3. I trained the model on 250 epochs. 
        Were you able to achieve the target model performance?
        No
        What steps did you take in your attempts to increase model performance?
        I reviewed previous evaluations and adjusted the model parameters in accordance, as stated above. 

    Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.
    Overall, the model performed at around 72% accuracy, over four different optimization attempts. I believe that a supervised machine learning model 
    may provide better results insofar as attaining accuracy. 
