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



--- Structure ---

Our repository includes 150 primary paragraphs. For each primary paragraph, there are three corresponding paragraphs representing neutrality, entailment, and contradiction, totaling 450 additional paragraphs.
