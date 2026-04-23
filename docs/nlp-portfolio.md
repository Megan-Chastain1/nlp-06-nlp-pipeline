# Applied Machine Learning Portfolio

Megan Chastain

2026-04

This page summarizes my work on **NLP** projects.


## NLP Techniques Implemented
Throughout the course a number of techniques were studied including:
- Tokenization of a word or sentence
    - Tokenization is the process of turning text into data points by breaking it down into foundational parts. Some words, 'stop words', are left out of the tokenization process because they occur frequently and don't provide value to the analysis. An example of a stop word is 'the'.
- Frequency analysis (unigram / n-gram)
    - Unigrams are single tokens, e.g. 'I', 'Love', 'NLP' and the frequency of their individual occurance.
    - N-grams are multiple(n) tokens that occur together and their frequency. An example would be 'I Love' or 'Love NLP'. This is also an example of a bigram.
- Text cleaning and normalization
    - This removes noise and standardizes the text. Stop words are removed as well as punctuation and capitalization. This makes it easier to break to find accurate frequencies, however some important information can be lost with the removal of capitalization.
- API-based text analysis (and JSON)
    - Using API text analysis an analyst can pull out specific categories of words, like people or places. An analyst can also break text into their parts of speech, identify language, and assign values to the text to determine if it's positive, negative, or neutral.
- Web scraping / content extraction from HTML
    - HTMLs provide lots of opportunities to analyze text content. An analyst can create a pipeline to extract text from a HTML website, tokenize it, and find frequencies of those tokens.
- Sentiment analysis (e.g., spaCy + SpacyTextBlob)
    - This assigns a numeric value to the text that can indicate if the text is positive, negative, or neutral.

## Systems and Data Sources
Different systems and data sources were used to implement the above techniques:

- Web pages
  - HTML web pages are coded with tags at the beginning and end of the text to designate what that text is: header, title, abstract, etc. To extract data an analyst needs to write a code to indentify the tags, pull the information from between them, and put that information in the correct column of a table.
- APIs
  - JSON is used to analyze APIs. JSON organizes data into arrays and objects. JSON requires a schema and keys to help organize the data, which is typically surrounded by {} brackets.
- datasets
- text documents
  - Plain text can be analyzed by turning it into a structured format using an EVTAL pipeline. This pipeline extracts data, validates it, transforms the structure of it, analyzes it, and loads that analysis into a separate well oraganized file.

All of these sources of data require the text to be preprocessed and cleaned. This includeds removing stop words, normalizing capitalization, converting words with suffixes to their root word (removing -ing, -ed, -es), and tokenizing the remaining text.

## Pipeline Structure (EVTL)

- Extract (from source): how data was collected
  - Data can be pulled from an HTML website, and API, or uploading a CSV or plain text document.
- Validate: structure/content checks performed
  - For JSON, the validate stage checks to make sure the document is in JSON structure.
  - For both JSON and HTML, the validate stage makes sure the expected elements are present and the data is usable.
- Transform: NLP processing steps
  - This step is where the cleaning and normalization of the text happns.
- Load (to sink): outputs (files, summaries, visualizations)
  - The results from the transform step are then put in a file and/or visualizations are created to see token frequency, important parts of the text, unigrams or n-grams, and sentiment values.

## Signals and Analysis Methods

- Word frequency
  - Word frequency was computed by breaking the text into tokens, counting how many times individual tokens appeared, then dividing that number by the total token count.
- Context or co-occurrence
- Keyword extraction
- Special signals
- Sentiment or subjectivity

## Insights
Describe what your analysis revealed:

patterns, trends, or notable findings
anything surprising or unexpected
what made the results useful or meaningful

## Representative Work
Provide links to 2–3 of your strongest projects.

For each project:

include a clickable link
provide 1–2 sentences describing what it does and why it is representative

## Skills
Be explicit about what you can do. Avoid general statements.

Examples:

Python data processing
working with text data
handling messy or inconsistent inputs
structuring repeatable pipelines
communicating results professionally with Markdown and visuals
