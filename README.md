# Shakespeare text generation using GPT

In this project, we want to train a transformer decoder on the tiny shakespeare dataset including 1 million characters at the character level and finally produce a text similar to it.

## Table of Contents

- [Shakespeare text generation using GPT](#shakespeare-text-generation-using-gpt)
- [Table of Contents](#table-of-contents)
- [How To Run](#how-to-run)
  - [Install Requirements](#install-requirements)
  - [Run Code](#run-code)
- [Results](#results)
- [License](#license)
- [Contact](#contact)

## How To Run

### Install Requirements

- If you want to run the script on the local machine, first run the following command to install the required libraries.
```
!pip install -r requirements.txt
```

- If you want to run the script on Google Colb, there is no need to install any library.

### Run Code

- In the first step, run the notebook "Bigram_(an_intro_to_GPT)" to familiarize with the dataset, tokenization and implementation of a very simple language model (bigram language model).

- In the second step, run the "Self_Attention" notebook to familiarize with the self-attention mechanism.

- In the last step, run the "bigram_SU_Final" script with the following command to train the transformer model and produce a text similar to tiny Shakespeare.
```
!wget https://raw.githubusercontent.com/karpathy/char-rnn/master/data/tinyshakespeare/input.txt

!python bigram_SU_final.py
```
If you don't have access to a local machine with GPU, it is suggested to use Google Colb because training the model on CPU will be very time consuming.

*Please read the file in the report folder before running the codes.*

## Results

The generated text file of 500 and 10,000 characters after 5,000 stages of model training, as well as the loss values in each step, are placed in the "result" folder.

The trained model has about 10.8 million parameters.

Despite the use of Google Colb GPU, it took about 1 hour to train the transformer model.

## License

This project is licensed under the MIT License.

## Contact

If you have any questions about the implementation of the project, you can send your questions to this email: alrzbqr@gmail.com
