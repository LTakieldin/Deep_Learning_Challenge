# Deep Learning Challenge
Alphabet Soup needs a model to help selecting applicants that have the best chance for success. Data was provided by Alphabet Soup's organization.

## Preprocess the Data
The first step is to do a bit of data cleaning for better intrepretation for our neural network. This included removing unecsesarry columns, identifying the target variable, splitting the data into test and train variables, implementing dummies for categorical data, and utilizing a scaler. The target variable was chosen to be the "IS_SUCCESSFUL" column while the rest of the columns become the feature variables. Columns 'EIN' and 'NAME' were determined to be irrelevant to our model.

## Compile, Train, Evaluate Model
The next step is to use TensorFlow to design the neural network. This includes setting up the input, hidden, and output layers, and training the model. Choosing number of epochs, neurons, and layers are also needed in optimizing the model. These were determined largely from trial and error.

## Optimize the Model
In an attempt to reach 75% accuracy, a number of methods were used. The steps taken in this example to optimize the model included changing the number of epochs neurons, adding hidden layers and dropout layers, changing activation functions(tanh, relu, sigmoid), and the optimizer while compliing the model ('adam'). During this process, a number of areas in our model were assesed. Eventually the chosen number of epochs were 100 although the accuracy did not significantly improve after the first 10 epochs. Two hidden layers and two dropout layers were also added to the improve the accuracy. The addition of dropout layers did significantly improve our model. More hidden layers were also added to improve accuracy but did not make a significant difference so the final amount of hidden layers were finalized at 2. Other unaffective methods were used to optimize the model such as changing the activation function to tanh, relu, and sigmoid, and changing the optimizer.

After many attempts, I was not able to reach the goal accuracy of 75%. However, I found that adding the dropout layers had the biggest positive impact on out model. Other methods that couldve been done include removing more columns, using hyperparameters to set the number of neurons more accurately, and/or using an early stoppng for our model.
