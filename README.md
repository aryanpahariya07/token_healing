# token_healing
# Token Healing Script

The Token Healing script is a Python program that performs token healing on text, correcting errors and improving the quality of the text data. It implements various techniques such as spelling and grammar correction, adding missing words, and removing duplicate words. The script utilizes libraries like GingerIt, spaCy, and transformers to execute the token healing operations.

## Prerequisites

Before running the script, ensure that you have the following prerequisites:

- Python 3.x
- Required libraries: torch, spacy, gingerit, transformers
- BERT pre-trained model: "bert-base-uncased"
- spaCy language model: "en_core_web_sm" (version 3.0.0)

## Installation

1. Clone the repository or download the script file to your local machine.

2. Install the required libraries using the following command:

pip install torch spacy gingerit transformers


3. Download the BERT pre-trained model by running the following command:

python -m transformers.cli.download bert-base-uncased


4. Download the spaCy language model by running the following command:

python -m spacy download en_core_web_sm-3.0.0


## Usage

1. Open a terminal or command prompt.

2. Navigate to the directory where the script file is located.

3. Run the script using the following command:

python token_healing.py


4. Enter the text you want to enhance when prompted.

5. The script will perform token healing operations and display the enhanced text as the output.

## Example

Here's an example usage of the script:

$ python token_healing.py
Enter text: Ths is an exmpl of inccrect txt.
Enhanced text: This is an example of incorrect text.


## Customization

If you want to customize the token healing techniques or extend the functionality, you can modify the corresponding functions in the script:

- `correct_spelling_and_grammar`: Handles spelling and grammar correction using the GingerIt library.
- `add_missing_words`: Implements BERT model-based word prediction to add missing words.
- `remove_duplicate_words`: Removes consecutive duplicate words using regular expressions.

Feel free to modify these functions to suit your specific requirements.

## Limitations

- The effectiveness of the token healing operations depends on the quality of the underlying models and libraries used.
- The script assumes English text. If you want to work with a different language, you may need to use an appropriate language model.
