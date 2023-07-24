
# Simple Deep Learning-Based Chatbot

This project is a simple deep learning-based chatbot that uses a three-layer neural network to predict the intent of user inputs. The model architecture consists of the following layers:

- **First Layer (Input Layer):**
  - Neurons: 128 neurons
  - Activation Function: Rectified Linear Unit (ReLU)

- **Second Layer (Hidden Layer):**
  - Neurons: 64 neurons
  - Activation Function: Rectified Linear Unit (ReLU)

- **Third Layer (Output Layer):**
  - Neurons: Number of intents (7 in this case)
  - Activation Function: Softmax

The model is trained to predict the intent of user messages from the following categories:

1. 'goodbye': Indicates a goodbye message.
2. 'greeting': Indicates a greeting message.
3. 'name': Indicates a message related to asking the chatbot's name.
4. 'options': Indicates a message inquiring about available options.
5. 'south_africa_facts': Indicates a request for facts about South Africa.
6. 'south_africa_info': Indicates a request for general information about South Africa.
7. 'thanks': Indicates a thank you message.

The training data contains labeled examples of user messages for each of the above intents. The model uses the Softmax activation function in the output layer to generate probability scores for each intent, and the intent with the highest probability is selected as the predicted intent.

## Getting Started

To run the chatbot locally, follow these steps:

1. Clone the repository to your local machine:

   ```
   git clone https://github.com/Pratik94229/Simple-Deep-Learning-Based-Chatbot.git
   ```
2. Create virtual enviorment:
   ```
   conda create -p venv python==3.8
   activate venv/
   ```

3. Install the required dependencies. The dependencies can be found in the `requirements.txt` file.

   ```
   pip install -r requirements.txt
   ```

4. Run the chatbot training notebook:

   ```
   chatbot_training_notebook.py
   ```

The chatbot will now be ready to interact with you based on the trained model.

5. Run application using
  ```
   python app.py
   ```

## Contributing

Feel free to modify the code and experiment with different models and techniques to improve the prediction accuracy.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

