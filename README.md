
## Spell Checker

This spell checker project is designed to identify and suggest corrections for misspelled words within a given text. It utilizes probabilistic models and various text processing techniques to provide accurate suggestions for misspelled words.

### Key Features:

1. **Finding Unique Words:** The project begins by extracting unique words from a large text corpus to build a vocabulary.

2. **Calculating Probability Distribution:** It computes the probability distribution of each word in the vocabulary based on its frequency in the corpus.

3. **Text Preprocessing:** Text preprocessing involves splitting, deleting, swapping, replacing, and inserting characters to generate possible corrections for misspelled words.

4. **Prediction:** The spell checker suggests corrections for misspelled words by considering the probability of each candidate word based on its presence in the vocabulary.

### Spell Checker Algorithm and Architecture

#### Algorithm Overview:
Peter Norvig's classic spell checker algorithm is a statistical approach to spell checking that suggests corrections for misspelled words based on their probability of occurrence in a given text corpus. The algorithm follows these key steps:

1. **Building Vocabulary:** Extracts unique words from a large text corpus to build a vocabulary.

2. **Calculating Probability Distribution:** Computes the probability distribution of each word in the vocabulary based on its frequency in the corpus.

3. **Text Preprocessing:** Implements text preprocessing techniques such as splitting, deleting, swapping, replacing, and inserting characters to generate possible corrections for misspelled words.

4. **Prediction:** Suggests corrections for misspelled words by considering the probability of each candidate word based on its presence in the vocabulary.

#### Architecture:
The spell checker project architecture can be divided into the following components:

1. **Data Acquisition:** Utilizes a large text corpus (e.g., the `big.txt` file) to build the vocabulary and calculate word probabilities.

2. **Text Preprocessing:** Includes functions for splitting words into parts, generating possible edits (deletions, swaps, replacements, insertions), and combining these edits to form candidate corrections.

3. **Prediction:** Determines the probability of each candidate correction based on the word probabilities calculated from the corpus.

4. **User Interface:** The spell checker can be accessed programmatically through functions like `spell_check(word)` and `spell_check_2(word)`, which return suggestions for misspelled words.

### Packages used and their usage:

1. **re**: Used for regular expression operations to extract words from the text corpus.

2. **pandas**: Utilized for organizing and processing data, particularly for creating data frames to store word probabilities and suggestions.

3. **tqdm**: Employed to display progress bars for iterative processes, enhancing the user experience by providing visual feedback on tasks such as building the vocabulary and calculating word probabilities.

### Credits:

- This project is inspired by Peter Norvig's classic spell checker algorithm.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
