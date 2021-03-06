# language_corrector
Contains methods used for language correction. It's in python. You need to have done:

`pip install --upgrade language-check`

in command line to install the language check library that supports this library. (This should take a few minutes.)

NOTE: language-check is dependent on languagetool being downloaded. Please download the desktop version from https://languagetool.org/, and unzip! (This may take around half an hour.)

## How to use:
Here's the easiest way to use it. See as follows:

```python
import language_corrector.grammar_checker
text = "Text to check grammar for."
print(language_corrector.grammar_checker.basic_grammar_check(text))
```

Make sure that GOOGLE_APPLICATION_CREDENTIALS is set to a file called key.json!

## Methods available:
- `basic_grammar_check()`: returns feedback based on the grammar check
- `long_suggestion_grammar_check()`: returns a list of each suggestion
- `num_of_errors()`: returns the number of errors
- `recommended_correction()`: returns a recommended correction
- `suggestion_dictionaries()`: returns a list of each suggestion, with dictionary values associated with the suggestion instead of a string.

# Translation methods available:
- `main.return_english()`: returns a grammar check in English
- `main.return_translation()`: returns a grammar check in a requested language

## How to install:
Download as a .zip file and unzip. Then, in command line, navigate to inside the language correction folder, then run:

`python setup.py install`
