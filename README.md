# Project Report Guideline

This page describes the guidelines to help you write up the final report of your project. Please note that the report should provide all the required information to evaluate your project, and at the same time, it should be concise and data-driven. I recommend you to follow these guidelines. Nonetheless, there is some flexibility, and you are welcome to add new sections as long as you remain within the general framework.

## Structure

Your final report **should not** exceed **12 single-spaced pages, using 11pt font**. 

**NO HANDWRITTEN** report will be accepted. 

The report must have the following structure:

- Title page
- Table of Contents
- Table of Figures
- Table of Abbreviations
- Abstract
- 1.Introduction
- 2.Background
- 3.Proposed Approach
- 4.Specification & Design
- 5.Implementation
- 6.Results & Evaluation
    * 6.1.Methodology
    * 6.2.Data set
    * 6.3.Results & Data Analysis
    * 6.4.Discussion
- 7.Future Work
- 8.Conclusions
- 9.References

The report must be written in **English**.

### 1. Introduction

A good **introduction** should tell the reader what the project is about (i.e., its purpose) without assuming any special knowledge and without introducing any specific material that might obscure his/her understanding. It should anticipate and combine the main points described in more detail in the rest of the document. It should also enthuse the readers about the project, to encourage them to read the whole report. Normally, an introduction comprises:

- the goal(s) of the project
- the intended audience or users of the work
- the scope of the project
- the strategy employed to carry out the project
- the assumptions on which the work relies on
- a summary of the important outcomes

### 2. Background

The **background section** aims to provide to reader the information that they cannot be expected to know, but which they will need to know in order to fully understand and appreciate the rest of the report. This section usually describes things such as:

- the wider context of the project
- the theory associated with the scope of the project
- the constraints on the approach to be adopted
- the methods and tools that the solution may be based on or use to solve the problem

### 3. Proposed Approach

Describe in reasonable detail the proposed approach you have used to address the problem. Give the pseudocode of the learning algorithm, including its general outline and the main equations. Trace through a concrete example of how the algorithm works. The example should be complex enough to illustrate all the essential aspects of the problem, but simple enough to be easily understood. If possible, an intuitively and meaningful example is better that one with meaningless symbols.

### 4. Specification & Design

The purpose of the **specification & design** section is to give to readers a clear picture of the system that will be created in terms of the required capability. A specification should tell readers what the system is required to do. The design gives them, the top-level details of how the system meets the requirements. It also points out constraints on the solution, that guided the decision making throughout the development process.

Describing what a software system does (i.e., specification) and how it does so (i.e., design) effectively usually means describing it from multiple viewpoints. In this case, each viewpoint must convey some information about the system that other viewpoints omit. Examples of possible viewpoints include:

- the user interface;
- the dynamic behavior of the system
- how data flows through the system
- what data types are implemented in the system
- what algorithms are implemented in the system
- the static architecture of the system, i.e., how the code is partitioned into modules

**It is strongly recommended to make extensive use of diagrams**

It is also important to justify the design of the system, for example, by discussing the implications of the constraints on the solution and on different design choices. Then, it should gives the reasons for making the choices the team did. Typically these implications will relate to the aims of the project and to aspects of it discussed in the background section.

### 5. Implementation

The **implementation** section is similar to the **specification & design** section. Therefore, it describes the system at a finer level of detail. This section is about the realization of the concepts and ideas presented in the previous sections. It can also describe any problems that may have arisen during the implementation and how the team dealt with them.

Please, do not attempt to describe all the code in the system, and do not include large pieces of code in this section. Instead pick out and describe just the pieces of code which, for example:

- are especially critical to the operation of the system
- illustrate a non-standard or innovative way of handling a problem

### 6 Results & Evaluation

This section should describe to what extent the goal of the project was achieved.

It should demonstrate that the system works as intended. It includes comprehensible summaries of the results of all critical tests that were carried out. 

This is also the place to describe the reasoning behind the tests to evaluate the system, what tests were executed, what the results are showing, and why these tests were selected.

All the results should be critically evaluated in the light of the tests, considering its strengths and weaknesses. It should present ideas to improve the solution in future works. **Remember**: no project is perfect, and even a project that has failed to deliver what was intended can achieve a good pass mark, if it is clear that the team have learned from their mistakes and difficulties.

This section also gives to team an opportunity to present a critical appraisal of the project as a whole. 

All these information should be distributed across the following subsections.

#### 6.1. Methodology

What criteria have you used to evaluate your proposed solution? What hypotheses do your experiment aims to test?

#### 6.2. Data set

What data set have you used to evaluate your solution? What are the dependent and the independent variables?

#### 6.3 Results & Data Analysis

Describe the quantitative results of your experiments. A graphical representation is usually better than tables. 

#### 6.4. Discussion

Are your hypotheses supported? What conclusions do the results support the strengths and weakness of your proposed solution compared to other existing approaches? How can the results be explained in terms of the underlying properties of the algorithm and/or the data?

### 7. Future Work

It is quite likely that by the end of your project you will not have  achieved all that you planned at the start; and in any case, your ideas  will have grown during the course of the project beyond what you could hope to do within the available time. 

This section exists to express the unrealised ideas. It is a way of  stating what you would like to have done if only you had not run out of time. A good future work section should provide a starting point for someone else to continue the work which you have begun.

### 8. Conclusions

This section summarizes the aims of project and it restates its main results. In other words, it describes what has been learned and what has been achieved. An effective set of conclusions should not introduce new material. Instead it should briefly draw out, summarize, combine, and reiterate the main points that have been made in the body of the report and present opinions based on them.

### 9. References

Include a comprehensive list of the references cited in the report. The references should be listed in alphabetical order of author's surname(s), and should give sufficient and accurate publication details. For example,

 - Date, CJ., 2000. An Introduction to Database Systems, 7th Edition. Addison-Wesley.
 - Verma, A., Pedrosa, L., Korupolu, M., Oppenheimer, D., Tune, E. and Wilkes, J., 2015. Large-scale cluster management at Google with Borg. 10th European Conference on Computer Systems.

---

## LaTeX template structure

* There is a TeX file for each chapter (introduction, background, proposed approach).
* Chapters files are placed under the directory _chapters_ and they are included in the report 
* **Figures** must be placed into the directory _figures_. It means that this is the directory where LaTeX will look for the graphics.
* Author's name and affiliation must be changed in the **report.tex** file
* Bib entries must be defined in the file **references.bib**.

### Generating the report

Open the file **report.tex** and compile it. This can be also done through the available _Makefile_. 

### LaTeX Writing Tips

* In your LaTeX document, avoid as much as possible to control the layout. Hence, you should never use \\ either you want to start a new paragraph or you don't but you should let LaTeX format the paper.
* Figures and tables are usually either placed on top or on bottom of the page, rarely in the middle. In other words, you should not force LaTeX to place figures or tables where you would like to see them.
* Tables' captions are placed above the table
* Figures' captions are placed under the figure.
* Tables should only have \toprule, \midrule, and \bottomrule. In other words, you should not use \hline in tables. 
* You can use [Table Generator](https://www.tablesgenerator.com) to help you design your tables.
* Always provide a label for your sections, figures, tables, and listings. 
* It's a good practice to prefix your labels using for instance the prefixes, fig:, sec:, tab:. This will be useful when an auto-complete suggests several entries and you need to select the one you want.
* Use ``\Cref`` to reference to figure, table, section, or listing. Thus, instead of writing for instance: ``as can be seen in Figure 1``, you write: ``as can be seen in~\Cref{fig:sample}``. 
* Use ``~`` put a space between a word and a reference or citation; e.g., in~cite{}. 
* Use ``\eg{}`` to write e.g., and ``\ie{}`` to write i.e., in your text. 
* Don't describe any acronym in your text. Instead, use \gls{your-acronym} and put its definition in the _abbreviations.tex_ file. For example 

% in the acronym file

```
\newacronym{ai}{AI}{Artificial Intelligence}
```

% in your text

```
\gls{ai} ... 
```

* Use \(\) or \[ \] to write math expressions
* Don't include neither the path nor the extension of the figure, when including one. 
* Set equations, floats and any other environments with commented blank lines. For example:
* Use ``\citeauthor{somebibentry}`` to include authors' names in the text.

## References

* D. Verna, *[Towards LATEX coding standards](http://www.tug.org/TUGboat/tb32-3/tb102verna.pdf),* TUGboat, vol. 32, no. 3, pp. 309–328, 2011.