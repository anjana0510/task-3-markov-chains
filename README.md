# Simple Text Generation with Markov Chains (Task-03)

This repository contains a Python script (markov_generator.py) that implements a simple text generation algorithm using Markov chains.

## Overview

The script takes a text corpus as input and builds a statistical model based on the sequence of characters within that text. The model learns the probability of a character following a given sequence of preceding characters (the "order" of the Markov chain determines the length of this preceding sequence).

Once trained, the model can generate new text by predicting the next character based on the previously generated characters, using the learned probabilities.

## Files

* markov_generator.py: The Python script containing the MarkovTextGenerator class and example usage.

## How to Use

1.  *Save the markov_generator.py file:* Download or save the provided Python code into a file named markov_generator.py.

2.  *Run the script:* You can run this script using a Python interpreter. Open your terminal or command prompt, navigate to the directory where you saved the file, and run:

    bash
    python markov_generator.py
    

3.  *Experiment with the code:*
    * *Text Corpus:* Modify the text_corpus variable in the if __name__ == "__main__": block to train the model on different text. You can use longer strings or load text from a file.
    * *Order:* Change the order variable when creating an instance of MarkovTextGenerator (e.g., order=1, order=3). Higher orders consider more preceding characters, potentially leading to more context-aware but also potentially more repetitive or data-dependent text.
    * *Length:* Adjust the length parameter in the generator.generate() method to control the length of the generated text.
    * *Start State:* Provide a start_state (a string of length equal to the order) to begin the text generation from a specific sequence of characters. If no start_state is provided, the generator will pick a random starting sequence from the training data.

## Example Output

When you run the script, you will see output similar to this (the exact output will vary due to the random nature of the generation):
