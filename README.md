
# deep-learning-challenge

# Neural Network Model to Alpahbet Soup Fundation

## Overview of the Analysis
The propose of the report is to explain if the model that we create with the data that Alphabet Soup Foundation give us have the accuracy neccesary to select the applicants for funding with the best chance of success in their ventures. For this, we make to models. 

The first neural network model use two hidden layers with 80 nodes and 30 nodes respectively, and in both layers we use the activation model "relu". finally, we use 100 epochs to test the model.

The second neural network model use three hidden layers with 100, 60 and 60 nodes respectively, and to the first layers, we use the activation model "relu" and to the others we used sigmoid activation model. Finally, we use 100 epochs to test the model.

## Results

* Data Preprocessing
    * Tarjet variables
    The tarjet varaible is "IS_SUCCESSFUL" that give you if the company was successful with your funding.
    * Features variables
    the features variables was:
        - Application Type
        - Affiliation
        - Classification
        - Use case
        - Organization
        - Statuss
        -Income AMT
        - Special Considerations
        - Ask AMT
    * Variables that we didnt used.
    The variables that we drop from the database was the name and the EIR, because you dont have relevant information from that.

* Compiling, Training and Evaluating the Model
    
    * Details of the models
        To the columns "APPLICATION TYPE" and "CLASSIFICATION" we considered like others everything that have less than 500 and 1000, respectively.
        Also, in this case we add to hidden layers and change the numbers of nodes for every hidden layers:
            - hidden_nodes_layer1=80
            - hidden_nodes_layer2=30
        Finnaly, the last thing that we change was the activation model. 
    * Achieve the tarjet?
        As a result, with this model we dont achieve the tarjet of 75% of accuracy. With this we cant say that we can trust in the model to give funding to the applicants.

    * improve the model performance
            to improve the model performance,  we considered the following changes in the model
            - change in the classfication columns, we take like other classification everything less than 500.
            - add to hidden layers and change the numbers of nodes. This, because i think that the data have a lot of details, so you need the necessary nodes and layers to analyse as many alternatives as posisible.
            - change the activation model. In this case we considered that only the first hidden layers was "relu", the others was "sigmoid" activation model. we change the activation model because i think that is the best model to predict  the probability of success.


## Summary
If you can see compare the graph of loss and accuracy for the models, both have a similar loss with 53% of the data,
![Alt text](<Loss Model.png>) ![Alt text](<Loos Model Optimized.png>)

Additionally, if we compate the accuracy graph, both models have similar accurary with 74%, this is insufficient to say that the model can predict the selection of good applicants.
![Alt text](<Accuracy Model.png>)  ![Alt text](<Accuracy Model Optimized.png>)

Finally, we evaluates the models, we have that both have a accurary of 72,6% and 57% of loss of the information. so you can conclude that the models dont have the accuracy neccesary to predict the success of the applicants.
 
