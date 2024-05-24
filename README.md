# Natural language processing course 2023/24: `Natural language inference dataset`

Paragraphs manually collected from ccGigafida and additional paragraphs, representing various semantic relations (neutrality, entailment, contradiction) to the primary paragraph, that were created using ChatGPT-4.

ccGigafida: https://www.clarin.si/repository/xmlui/handle/11356/1035 

This dataset was created by Digitalke (public acronym/name: ul-fri-nlp-course-project-digitalke).
Link to our repository: https://github.com/UL-FRI-NLP-2023-2024/ul-fri-nlp-course-project-digitalke
------------------------------------------------------------------------------------------------------------------------

--- Overview ---

After downloading the ccGigafida corpora, it was first preprocessed in Python. Preprocessing included extracting relevant textual content, ignoring metadata, headers, footers, non-textual elements and any unnecessary whitespace.

The files were seperated into three different sections, and then K-means clustering was used to find the most common themes in each section. After that, the most representative paragraphs for each cluster were manually selected. Then, we came up with creative prompts for each paragraph to bring out different semantic relations (following the SI-NLI Guidelines).

We then fed these prompts to ChatGPT-4 to create corresponding paragraphs.

The created paragraphs were meticulously reviewed and annotated to ensure a clear relationship with the original text. Paragraph pairs were randomly selected and provided to both ChatGPT-3.5 and ChatGPT-4 to evaluate which model performs better in identifying the relationships between the paragraphs.

A comprehensive statistical analysis was conducted to compare the performance of both models.


--- Structure ---

Our repository includes 150 primary paragraphs. For each primary paragraph, there are three corresponding paragraphs representing neutrality, entailment, and contradiction, totaling 450 additional paragraphs. These are saved directly in folder Paragraphs and also in the original Word file, which can be accessed through our repository.

The entire dataset consists of the following parts:
- "Paragraphs" - the whole dataset, including original extracted paragraphs, creative prompts and three paragraphs expressing neutrality, entailment and contradiction, for each of the original paragraph respectively.
- "evaluation-ChatGPT.xlsx" - statistic analysis comparing the performance of ChatGPT-3.5 and ChatGPT-4 in recognizing the semantic relationship between paragraphs.
- "report/code" - contains both codes used for preprocessing and K-means clustering.

