---
layout: default
---


## Comprehensive Analysis of Character-Agency through Computer-based Tools

### Abstract

><i class="fa fa-quote-left fa-2x fa-pull-left fa-border"></i>We tell stories to teach cultural norms,
>to entertain, and to help create shared perspectives (Boyd et al. 1)"


Literature shapes cultural norms and heritage through language. Recent studies focus on gender in text analysis, with computerized methods like NLP offering efficient insights[^1]. Language reflects and reinforces gender stereotypes and power dynamics, but can also be a tool for resistance and subversion. Research shows how linguistic features contribute to maintaining gender-based inequalities. The combination of agency and gender analysis using computerized tools remains relatively unexplored. The thesis aims to investigate the correlation between fictional character agency, gender, and author gender, using the Gutenberg Corpus as research data. By utilizing the tools LIWC, Lingualyzer and BookNLP this research study intents to highlight the difficulties and challenges but also the advatages of using computationalized tools to analyze social concepts like agency.

<hr>

### Content

<ul class="fa-ul">
  <li><i class="fa-li fa fa-solid fa-arrow-right"></i><a href="#data-and-results">Data and Results</a></li>
  <li><i class="fa-li fa fa-solid fa-arrow-right"></i><a href="#challenges-and-biases">Challenges and Biases</a></li>
  <li><i class="fa-li fa fa-solid fa-arrow-right"></i><a href="#references">References</a></li>
  <li><i class="fa-li fa fa-solid fa-arrow-right"></i><a href="#resources">Resources</a></li>
  <li><i class="fa-li fa fa-solid fa-arrow-right"></i><a href="#contact">Contact</a></li>
</ul>

<hr>

#### Data and Results


For this study, a small subset of the Gutenberg Project corpus was used, which excluded non-fiction, poetry, drama, and other genres. The focus was solely on novels and short stories. The decision to exclude other genres was based on meta-data and previous research by Nagaraj and Kejriwal (2020) to avoid biased or inconclusive results. The subset's adherence to the criteria was verified through random samples, ensuring the study's reliability and validity. Due to limited resources, a focused approach was necessary, and detailed examinations of all authors' texts and genres were eliminated. This method was chosen to ensure a representative and unbiased sample for the study.


<b>LIWC</b>

The Linguistic Inquiry and Word Count (LIWC) software, developed by renowned researcher James W. Pennebaker, is a widely utilized tool in the fields of psychology, sociology, and communication studies for the quantitative analysis of written texts. While LIWC offers invaluable insights, it is important to acknowledge its limitations, such as the presence of predetermined categories and a primary focus on textual content rather than broader contextual or qualitative considerations. Noteworthy features of LIWC include a narrative arc analysis function and the ability to process large volumes of text without the need for prior programming expertise. In essence, LIWC serves as a powerful instrument for examining language usage patterns and their potential impact on human behavior; however, caution must be exercised in its application to ensure the accuracy and reliability of the results.
<img src="images/FemaleHighAgencyNarrative Arc.JPG" alt="female high agency narrative arc">
In my investigation into agency within narrative structures at both macro and micro levels, each text was segmented into five distinct sections utilizing the LIWC software to facilitate a more thorough comparative analysis. The resultant data was then formatted in .csv or .xlsx documents, facilitating the aggregation of findings into a cohesive report. I employed the default English language dictionary within LIWC for further analytical purposes, focusing on a single work per author and producing graphical representations for enhanced interpretation. The outcomes of this analysis shed light on the underlying narrative frameworks present in the selected literary works.
<img src="images/MaleHighAgencyNarrativeArc.JPG" alt="male high agency narrative arc">
The data obtained reveals a notable discrepancy in the levels of agency displayed by female authors compared to their male counterparts. Specifically, female authors demonstrated a propensity towards employing a greater number of positive emotion words and emotional language overall in their writing. Furthermore, it was observed that female authors maintained a higher average positive tone and a slightly elevated negative tone in their texts as compared to male authors. Interestingly, male authors exhibited a higher frequency of male references, while female authors leaned towards incorporating more female references in their work. Additionally, the analysis highlighted a distinction in pronoun usage between genders, with male authors favoring the use of first-person singular pronouns and female authors displaying a preference for third-person singular pronouns. Notably, both male and female authors employed the pronoun "they" less frequently, albeit with a marginally higher usage rate among male authors.
<img src="images\LIWCAverageEmotionTone.png" alt="average tone graph">


<b>Lingualyzer</b>

Lingualyzer, a computational linguistic tool developed by Guido M. Linders and Max M. Louwerse with computational implementation from Kiril O. Mitev, is specifically designed for the analysis of multilingual and multidimensional texts. This tool serves as a valuable resource for researchers and analysts seeking to accurately analyze large volumes of text data in various languages, thereby facilitating a more comprehensive understanding of content (Linders and Louwerse 2). Despite some limitations such as the absence of batch processing and a plethora of features that may at times overwhelm users, Lingualyzer prioritizes consistency and usability for commonly used languages. The developers are currently exploring the possibility of incorporating batch processing to cater to a broader audience, as processing documents individually can be inconvenient (Linders and Louwerse 23).
In order to adhere to Lingualyzer's character limit of 40,000, longer text files were segmented using the git bash software with the command git split. Similar to BookNLP, Lingualyzer requires a few minutes for analysis, contingent upon factors like internet connection speed. For this study, a single work per author was selected for analysis due to time constraints. Analysis data from Lingualyzer was made available for download in txt format on the Lingualyzer website and was subsequently imported into Excel for organization and visualization to ensure consistency and ease of manipulation.

The results of the study revealed that texts with lower counts of passive voice tend to exhibit higher agency, particularly evident in works such as Wuthering Heights and The Life and Death of Mr. Badman for female and male authors respectively. Furthermore, the analysis highlighted that novels such as The Tale of Mr. Jeremy Fisher and The Raven had the lowest passive voice counts. Additionally, there were notable variations in verb types, occurrences, and ratios observed across different works, providing insights into the stylistic choices of various authors. For instance, works like Wuthering Heights and The Life and Death of Mr. Badman demonstrated higher verb-noun ratios, indicating a particular emphasis on action within the narrative. Conversely, texts like Brownes Folly and The Tale of Mr. Jeremy Fisher exhibited lower pronoun-noun ratios, suggesting a different approach to character depiction and narrative structure.


<b>BookNLP</b>

In contrast to LIWC and Lingualyzer, the BookNLP pipeline, developed by David Bamman, is tailored for users with a programming background. BookNLP is a natural language processing pipeline specifically designed for the analysis and processing of longer documents, extracting linguistic features such as character names, locations, relationships, and actions to enhance the understanding and analysis of literary texts. Employing a range of language processing techniques like named entity recognition, part-of-speech tagging, and dependency parsing, BookNLP utilizes pre-trained models and data sets focused on long-format texts to enhance the accuracy of analysis. The application of BookNLP spans various research projects in fields such as literary analysis, digital humanities, and text mining, making it freely available for academic and research purposes through its GitHub repository.
During the installation process of BookNLP on Windows, known technical challenges were encountered, leading to the utilization of Google Colab servers for computational analysis. However, limitations on run time and RAM prevented concurrent processing of multiple files, necessitating a sequential analysis on a per-author basis. The appendices contain the code used for configuring and executing BookNLP, with data stored both on Google Drive and the local machine. After data collection, a conversion into XLSX format facilitated statistical interpretation and visualization while generating word clouds for characters based on values of mod, poss, patient, and agent for further analysis in later sections.
Analysis of the BookNLP data indicated a higher prevalence of male characters compared to female characters on average, with female authors favoring female characters and male authors tending towards male characters. Usage of gender-neutral pronouns was limited for both genders, albeit with male authors exhibiting a slightly higher frequency. Notably, a singular occurrence of ze/zem/zir/hir pronouns was identified, likely a false positive. Divergence in results from the BookNLP and LIWC analyses could stem from the relatively small sample size in the former, consisting of a single text per author. Female characters demonstrated a slightly greater dominance in sentences, assuming roles as agents, possessions, and patients, aligning with hypotheses suggesting a higher propensity for females to act as patients over agents.
<img src="images\wordcloudGritzelmod.png" alt="word coud modifier">
Specific characters like Fan from William Henry Hudson’s "Fan" scored highest in both agent and patient roles, while Grizel from James Matthew Barrie’s "Tommy and Grizel" excelled in modifier and possessions categories. Negative connotations associated with Grizel contradicted assumptions linking male characters to negative emotions. However, BookNLP's unreliability in accurately classifying first names was evident when Grizel was mistakenly tagged as male, highlighting limitations in gender recognition accuracy. Instances of Fan as an agent linked to intransitive verbs could impact reader comprehension, influencing the concept of agency portrayed in the text. Challenges in interpreting BookNLP results are acknowledged due to the tool's inherent limitations, to be further elaborated on in forthcoming sections. Ultimately, the analysis upholds the initial research hypothesis, revealing distinctions in the creation and comprehension of male and female characters that could spark future research endeavors.


<hr>

### Challenges and Biases

The utilization of computational tools in language and text analysis has proven to be highly beneficial, particularly in the realm of person-entity recognition and linking within literary texts. However, traditional methods have often proven inadequate due to the intricate and nuanced nature of character names and descriptions in narratives. As a result, researchers have sought innovative approaches that combine established techniques with machine learning algorithms specifically tailored to literary data (Lajewska and Wróblewska 8–9). In recent years, numerous studies have been undertaken to explore effective strategies for character detection and analysis in literary texts, especially when employing a quantitative methodology. These studies aim to uncover novel techniques for character detection and analysis that can facilitate tasks such as sentiment analysis, character relationship mapping, and plot analysis. In light of the ongoing digital transformation reshaping how we engage with and analyze texts, the development of more sophisticated tools and techniques is imperative to enhance our comprehension of literary works (Vala et al. 769).

Research in the fields of natural language processing and artificial intelligence has been predominantly focused on the development of machine learning algorithms capable of processing and analyzing textual data with efficacy. These algorithms rely on extensive annotated text datasets for training and learning purposes. The process involves manually labeling text samples with relevant tags or labels to enable algorithms to identify patterns and make accurate predictions. The quality and quantity of annotated data significantly influence the performance and effectiveness of machine learning algorithms, underscoring the importance of meticulous data curation to enhance model reliability (Soni et al. 8–9).

While computational tools such as genderize.io have been instrumental in inferring gender from first names, their accuracy can be further enhanced by incorporating additional factors or methodologies into the analysis. Researchers must remain vigilant in ensuring the credibility of such tools, as human biases may inadvertently permeate the analysis process. Paul Sebo's research on evaluating name-to-gender inference services underscores the complexity and challenges inherent in relying on names as proxies for gender identification, especially given the multicultural diversity of names and the potential for misgendering. Greater transparency, accountability, and continuous refinement in the development and application of gender detection tools are essential to improving accuracy and inclusivity (Sebo, “Performance of gender detection tools: a comparative study of name-to-gender inference services” 419–20).

Emphasizing the inherent limitations of computational tools, an example involving the misclassification of a character's gender by a tool like BookNLP serves as a poignant reminder of the complexities inherent in simplifying human concepts for algorithmic processing. Accessibility issues also come to the forefront, exemplified by the challenges posed by different computational tools with varying levels of usability and availability. Subsequently, the thesis delves into the nuances of addressing biases and assessing creative works quantitatively, aiming to unveil a more objective approach to evaluative processes. The incorporation of computer-analytic developmental scales for assessing writing proficiency represents a notable advancement in streamlining and standardizing the evaluation of students' writing skills, demonstrating strong correlations with established measures of writing ability (Burdick et al. 273–77).

Further studies exploring the influence of gender and ethnicity on writing performance shed light on potential biases and societal expectations that may impact evaluative judgments. The research underscores the need for educators and evaluators to remain cognizant of these biases and strive for fair and impartial assessments of creative works, fostering a more inclusive and equitable evaluation process. Lastly, by leveraging computational tools to mitigate biases and enhance objectivity in evaluative processes, the author endeavors to ensure that assessments of creative works are robust, reliable, and reflective of true merit.

<hr>

### References

Burdick, Hal; Swartz, Carl W.; Stenner, A. Jackson; Fitzgerald, Jill; Burdick, Don; Hanlon, Sean T. (2013): Measuring Students’ Writing Ability on a Computer-Analytic Developmental Scale: An Exploratory Validity Study. In: Literacy Research and Instruction 52 (4), S. 255–280. DOI: 10.1080/19388071.2013.812165.

Lajewska, Weronika; Wróblewska, Anna (2021): Protagonists' Tagger in Literary Domain -- New Datasets and a Method for Person Entity Linkage.

Linders, Guido M.; Louwerse, Max M. (2023): Lingualyzer: A computational linguistic tool for multilingual and multidimensional text analysis. In: Behavior research methods. DOI: 10.3758/s13428-023-02284-1.

Nagaraj, Akarsh; Kejriwal, Mayank (2022): Dataset for studying gender disparity in English literary texts. In: Data in brief 41, S. 107905. DOI: 10.1016/j.dib.2022.107905.

Sebo, Paul (2021): Performance of gender detection tools: a comparative study of name-to-gender inference services. In: Journal of the Medical Library Association : JMLA 109 (3), S. 414–421. DOI: 10.5195/jmla.2021.1185.

Soni, Sandeep; Sihra, Amanpreet; Evans, Elizabeth F.; Wilkens, Matthew; Bamman, David (2023): Grounding Characters and Places in Narrative Texts. [Online verfügbar](http://arxiv.org/pdf/2305.17561v1)

Vala, Hardik; Jurgens, David; Piper, Andrew; Ruths, Derek: Mr. Bennet, his coachman, and the Archbishop walk into a bar but only one of them gets recognized: On The Difficulty of Detecting Characters in Literary Texts. In: Lluís Màrquez, Chris Callison-Burch und Jian Su (Hg.): Proceedings of the 2015 Conference on Empirical Methods in Natural Language Processing. Proceedings of the 2015 Conference on Empirical Methods in Natural Language Processing. Lisbon, Portugal. Stroudsburg, PA, USA: Association for Computational Linguistics, S. 769–774.


<hr>

#### Resources

<i class="fa-regular fa-scroll fa-3x fa-pull-left"></i>

[Project Repository](https://gitlab.rlp.net/limmerhe/decoding-gender-in-fictional-character-development)\
[LIWC](https://www.liwc.app/)\
[Lingualyzer](https://lingualyzer.com)\
[BookNLP](https://github.com/booknlp/booknlp)

<hr>

### Contact

#### Lisa Immerheiser (she/her)

{% include sharing.html %}

<b>This website was created  as part of a master thesis at the Johannes Gutenberg-Universität Mainz within the degree program Digital Humanities (Digitale Methodik in den Geistes- und Kulturwissenschaften)</b>


### [^1]: Footnotes

Lajewska, Weronika; Wróblewska, Anna (2021): Protagonists' Tagger in Literary Domain -- New Datasets and a Method for Person Entity Linkage.

Lucy, Li; Bamman, David (2021): Gender and Representation Bias in GPT-3 Generated Stories. In: Proceedings of the Third Workshop on Narrative Understanding. Stroudsburg, PA, USA. Stroudsburg, PA, USA: Association for Computational Linguistics.

Nagaraj, Akarsh; Kejriwal, Mayank (2022): Dataset for studying gender disparity in English literary texts. In: Data in brief 41, S. 107905. DOI: 10.1016/j.dib.2022.107905.