# Preface {-}





<p style="font-weight:bold; color:blue;">BOOK PROPOSAL DRAFT</p>

> The journey of a thousand miles begins with one step.
>
> --- [Lao Tzu](https://en.wikipedia.org/wiki/Laozi)

<div class="rmdkey">
<p>The essential questions for the preface are:</p>
<ul>
<li>What is the rationale for this textbook?</li>
<li>What are the aims and the approach taken in this textbook?</li>
<li>How is the textbook designed to support attaining these aims?</li>
<li>What is needed to get started?</li>
</ul>
</div>

This chapter aims to provide a brief summary of current research trends that form the context for the rationale for this textbook. It also provides instructors and readers an overview of the aims and approach of the textbook, a description of the main components of each section and chapter, a guide to conventions used in the book, and a summary of the supporting resources available. Additionally information on setting up your computing environment and where to seek support is included.  

<!-- To wrap up, I will provide an overview of the rest of the textbook highlighting the learning goals, the structure of the textbook, and how this structure will support a robust knowledge of what text analysis is, why it is used, and how to conduct original research. -->

## Rationale {-}

In recent years there has been a growing buzz around the term 'Data Science' and related terms; data analytics, data mining, *etc*. In a nutshell data science is the process by which an investigator leverages statistical methods and computational power to uncover insight from machine-readable data sources. Driven in large part by the increase in computing power available to the average individual and the increasing amount of electronic data that is now available through the internet, interest in data science has expanded to virtually all fields in academia and areas in the public sector. 

<!-- This textbook is an introduction to the fundamental concepts and practical programming skills from Data Science that are increasingly employed in a variety of language-centered fields and sub-fields applied to the task of quantitative text analysis. It is geared towards advanced undergraduates, graduate students, and researchers looking to expand their methodological toolbox. -->

This textbook is an introduction to the fundamental concepts and practical programming skills from data science applied to the task of quantitative text analysis. The intended readership for this textbook is primarily undergraduate students but may also be applicable to graduate students and researchers looking to expand their methodological toolbox. This textbook aims to meet the growing interest in quantitative data analysis methods taking hold across linguistics subfields and language-informed disciplines (digital humanities, political science, economics, *inter alia*). To ensure that this resource is accessible to a wide variety of students and researchers it does not assume a background in linguistics. Additionally, some readers interested in the aforementioned disciplines may lack experience with and/ or feel hesitant towards statistical methods and/ or programming. To make this textbook attractive to novices in quantitative text analysis methods, I will make no assumptions about the reader's experience with quantitative data analysis or programming, in general, or programming with the statistical programming language R, in particular.

## Aims {-}

<!-- From this textbook readers will gain the ability to: 1) interpret, assess, and contextualize findings based on textual data (__Data literacy__), 2) conduct original text analysis research including design, implementation, interpretation, and communication (__Research skills__), and 3) produce original research in the programming language R and learn collaborative workflows using current technologies that support reproducible research (__Programming skills__). -->

This textbook aims to develop the reader's proficiency in three main areas:

__Data literacy__: the ability to interpret, assess, and contextualize findings based on data. Throughout this textbook we will explore topics which will help you understand how data analysis methods derive insight from data. In this process you will be encouraged to critically evaluate connections across linguistic and language-related disciplines using data analysis knowledge and skills. Data literacy is an invaluable skillset for academics and professionals but also is an indispensable aptitude for in the 21st century citizens to navigate and actively participate in the 'Information Age' in which we live [@Carmi2020].

__Research skills__: the ability to conduct original research, communicate findings, and make meaningful connections with findings in the literature of the field. This target area does not differ significantly, in spirit, from common learning outcomes in a research methods course: identify an area of investigation, develop a viable research question or hypothesis, collect relevant data, analyze data with relevant statistical methods, and interpret and communicate findings. However, working with text will incur a series of key steps in the selection, collection, and preparation of the data that are unique to text analysis projects. In addition, I will stress the importance of research documentation and creating reproducible research as an integral part of modern scientific inquiry [@Buckheit1995]. 

__Programming skills__: the ability to implement research skills programmatically and produce research that is replicable and collaborative. Modern data analysis, and by extension, text analysis is conducted using programming. There are various key reasons for this: (1) programming affords researchers unlimited research freedom --if you can envision it, you can program it. The same cannot be said for off-the-shelf software which is either proprietary or unmaintained --or both. (2) Programming underlies well-documented and reproducible research --documenting button clicks and menu option selections leads to research which is not readily reproduced, either by some other researcher or by your future self! (3) Programming forces researchers to engage more intimately with the data and the methods for analysis. The more familiar you are with the data and the methods the more likely you are to produce higher quality work.

<!-- ADD: 

- ... Many textbooks...
- what makes this textbook unique (competition points)
  - developing skills/habits/ perspective/ think like quantitative data analysis
  - underscore the importance of framing research and developing a research plan before embarking on a project
  - survey common methods in text analysis which apply to a wide variety of fields, not just linguistics
  - emphasize breadth over depth in terms of statistical approaches, point to further reading 
  - reproducibility

-->


<!-- Many textbooks on doing 'Data Science', even those that have a domain-centric approach, such as text analysis, tend to focus on the 'tidy' approach, seen in Figure \@ref(fig:tidy-workflow-img) from @Wickham2017.  -->


<!-- However these resources tend to underrepresent the importance of establishing a research question and implementation plan. A big part, or perhaps the biggest part of doing quantitative research, and research in general is what is the question to be addressed. I think a central advantage to this coursebook for language researchers is to thread the project goals from a conceptual point of view without technical implementation in mind first. Then, after establishing a viable vision about what the data should look like, how it should be analyzed, and how the analysis will contribute to knowledge in the field, we can move towards implementing these preliminary formulations in R code in a reproducible fashion. In essence this approach reflects [the classic separation between content and format](https://en.wikipedia.org/wiki/Separation_of_content_and_presentation) –the content of our research should precede the format it should or will take. -->

## Resources {-}

This textbook includes three resources to support learning in the areas of Data literacy, Research skills, and Programming skills in a systematic chapter-related fashion: 1) the textbook itself which includes prose discussion, figures/tables, R code, and thought and practical exercises, 2) a companion website "[Text as Data Resources](https://lin380.github.io/tadr/)" which includes programming tutorials and demonstrations to develop and augment the reader's recognition of how programming strategies are implemented, and 3) a [GitHub repository](https://github.com/lin380) which contains both a set of interactive R programming lessons ([Swirl](https://github.com/lin380/swirl)) and [lab exercises](https://github.com/stars/francojc/lists/labs) which guide the reader through practical hands-on programming applications.

<!-- ADD: 

- more detailed resources description here?

-->


## Structure {-}

In __Part I "Foundations"__ the aims are to: 1) provide an overview of quantitative research and their applications, by both highlighting visible applications and notable research in various fields, 2) consider how quantitative research contributes to language research, and 3) layout the main types of research and situate quantitative text analysis inside these. 

In __Part II "Orientation"__ we will build up a framework to contextualize quantitative data analysis using the Data to Insight (DIKI) Hierarchy in Figure \@ref(fig:diki-hierarchy) ^[Adapted from @Ackoff1989]. 

<div class="figure" style="text-align: center">
<img src="images/02-introduction/diki-hierarchy-paper.png" alt="Data to Insight Hierarchy (DIKI)" width="90%" />
<p class="caption">(\#fig:diki-hierarchy)Data to Insight Hierarchy (DIKI)</p>
</div>

The DIKI Hierarchy highlights the stages and intermediate steps required to derive insight from data. [Chapter 2 "Understanding data"](#understanding-data-chapter) will cover both Data and Information covering the conceptual topics of populations versus samples and how language data samples are converted to information and the forms that they can take. In [Chapter 3 "Approaching analysis"](#approaching-analysis-chapter) I will discuss the distinction between descriptive and analytic statistics. In brief they are both important for conducting data analysis, but descriptive statistics serve as a sanity check on the dataset before submitting it to interrogation --which is the goal of analytic statistics. We will also cover some of the main distinctions between analytics approaches including inference-, exploration-, and prediction-based methods. With a fundamental understanding of data, information, and knowledge we will then move to [Chapter 4 "Framing research"](#framing-research-chapter) where we will discuss how to develop a research plan, or what I will call a 'research blueprint'. At this point we will directly address Research Skills and elaborate on how research really comes together; how to bring yourself up to speed with the literature on a topic, how to develop a research goal or hypothesis, how to select data which is viable to address the research goal or hypothesis, how to determine the necessary information and appropriate measures to prepare for analysis, how to perform diagnostic statistics on the data and make adjustments before analysis, how to select and perform the relevant analytic statistics given the research goals, how to report your findings, and finally, how to structure your project so that it is well-documented and reproducible. 

__Part III "Preparation"__ and __Part IV "Analysis"__ serve as practical and more detailed guides to the R programming strategies to conduct text analysis research and as such develop your Programming Skills. In [Chapter 5 "Acquire data"](#acquire-data-chapter) I will discuss three main strategies for accessing data: direct downloads, Automatic Programming Interfaces (APIs), and web scraping. In [Chapter 6 "Curate data(sets)"](#curate-datasets-chapter) I will outline the process for converting or augmenting the acquired data or dataset into a (more) structured format, therefore creating information. This will include organizing linguistic and non-linguistic metadata into one dataset. In [Chapter 7 "Transform datasets"](#transform-datasets-chapter) I describe how to work with a curated dataset to derive more detailed information and appropriate dataset structures that are appropriate for the subsequent analysis. 

[Chapters 8 "Inference"](#inference-chapter), [9 "Prediction"](#prediction-chapter), and [10 "Exploration"](#exploration-chapter) focus on different categories of statistical analysis each associated with distinct research goals. Inference deals with analysis methods associated with standard hypothesis-testing. This will include some common statistical models employed in text analysis: chi-squared, logistic regression, and linear regression. Prediction covers methods for modeling associations in data with the aim to accurately predict outcomes using new textual data. I will cover some standard methods for text classification including Näive Bayes, *k*-nearest neighbors (*k*-NN), and decisions tree and random forest models. Exploration covers a variety of analysis methods such as association measures, clustering, topic modeling, and vector-space models. These methods are aligned with research goals that aim to interpret patterns that arise in from the data itself.

__Part V "Communication"__ covers the steps in presenting the findings of the research both as a research document and as a reproducible research project. Both research documents and reproducible projects are fundamental components of modern scientific inquiry. On the one hand a research document, covered in Chapter [11 "Reporting"](#reporting-chapter), provides readers a detailed summary of the main import of the research study. On the other hand making the research project available to interested readers, covered in Chapter [12 "Collaboration"](#collaboration-chapter), ensures that the scientific community can gain insight into the process implemented in the research and thus enables researchers to vet and extend this research to build a more robust and verifiable research base.


<!--


### Learning goals {-}

From this textbook readers will gain the ability to: 1) interpret, assess, and contextualize findings based on textual data (Data literacy), 2) conduct original text analysis research including design, implementation, interpretation, and communication (Research skills), and 3) produce original research in the programming language R and learn collaborative workflows using current technologies to support reproducible research (Programming skills). 

__Data Literacy (DL):__ 

1. ability to understand and apply data analysis to derive insight from data
2. ability to understand and apply data knowledge and skills across linguistic and language-related disciplines

__Research Skills (RS):__  

1. identify an applicable area of investigation in a linguistic or language-related field
2. develop a viable research question or hypothesis
3. assess, acquire, and document data
4. curate and transform data for analysis
5. select and apply relevant analysis method
6. interpret and communicate findings

__Programming Skills (PS):__ 

1. demonstrate proficiency to implement research with R (RD points 3-5)
2. demonstrate ability to produce collaborative and reproducible research using R, RStudio, and GitHub

In each chapter of this coursebook specific learning objectives will be specified that target these learning outcomes so it is clear what we are doing and why were are doing it.

### Prerequisites {-}

This coursebook is aimed at students that have some background in language-related studies or linguistics with a desire to expand their methodological toolbox. It does not assume a strong background in these areas, however. Furthermore, I will make no assumptions about students' experience with programming in general, or programming with R, in particular. 

You will need reliable access to the internet and a computer to work with the code in this coursebook and the code found in the accompanying resource site ([tadr](https://lin380.github.io/tadr/)). 

### Programming {-}

Programming is the backbone for modern quantitative research. Here are some of the reasons to program:

- *Flexibility* Graphical User Interface (GUI) based software is inherently limited. What you see is what you get. If you have another need, you need to find a tool. If another tool does not implement what you think you need, you are out of luck.
- *Transparency* By taking a programming approach to research analysis you make your decisions explicit and leave a breadcrumb trail to everything you do.
- *Reproducibility* What you do will be clearer to you but also allow you to share the process with others (including your future self!). Insight grows much faster when exposed to light. Sharing your research with collaborators or on sites such as GitHub or BitBucket brings makes your work visible and accessible to the world. Reproducibility is gaining momentum and is fueled by programmatic approaches to research.

R is a popular programming language with statisticians and was adopted by many other fields in natural and social sciences. There are various reasons why using R for this coursebook is a good choice:

- *One stop shopping* Once known specifically as a statistical programming language, R can now be a round trip tool to acquire, curate, transform, visualize, *and* statistically analyze data. It also allows for robust communication in reports and data and analysis sharing (reproducibility).
- *You are not alone* There is a sizable R programming community, especially in academics. This has two tangible benefits; first, you will likely be able to find user contributed R packages that will satisfy many of the more sophisticated programming goals you will have and second, you will be able to get answers to any of your programming questions on popular sites like StackOverflow.
- *RStudio* RStudio is the envy of many other programmers. It is a very capable interface to R and provides convenient access powerful tools to allow you to be a more efficient and productive R programmer.

## Coursebook structure {-}

This coursebook is divided into four parts:

1. In "Foundations", an environmental survey of quantitative research across disciplines and orient language-based research is provided. 
2. "Orientation" aims to build your knowledge about what data is, how text is organized into datasets, what role statistics play in quantitative research and the types of statistical approaches that are commonly found in text analysis research, and finally how to develop a research question and a research blueprint for conducting a quantitative text analysis research project. 
3. "Preparation" covers a variety of implementation approaches for each stage for deriving a dataset ready for statistical analysis which includes acquiring, curating, and transforming data. 
4. "Analysis" elaborates various statistical approaches for data analysis and contextualizes their application in for different types of research questions and aims. 

-->

## Conventions {-}

This textbook is about the concepts for understanding and the techniques for doing quantitative text analysis with R. Therefore there will be an intermingling of prose and code presented. As such, an attempt to establish consistent conventions throughout the text has been made to signal the reader's attention as appropriate. 

In terms of prose, key concepts will be signaled using __bold__. As we explore concepts, R code itself will be incorporated into the text. 

For example, the following text block shows actual R code and the results that are generated when running this code. Note that the hashtag `#` signals a **code comment**. The code follows within the same text block and a subsequent text block displays the output of the code.


```r
# Add 1 plus 1
1 + 1
#> [1] 2
```

Inline code will be used when code blocks are short and the results are not needed for display. For example, the same code as above will sometimes appear as `1 + 1`. 

When necessary meta-description of code will appear. This is particularly relevant for R Markdown documents. 

````clike
```{r test-code}
1 + 1
```
````

There is a series of text blocks that will be used to signal the reader's attention to: *key points*, *concept questions*, *case studies*, *swirl lessons*, *programming tutorials*, *lab exercises*, *tips*, and *warnings*.  

Key points summarize the main points to be covered in a chapter or a subsection of the text.

<div class="rmdkey">
<p>The essential questions for the preface are:</p>
<ul>
<li>What is the rationale for this textbook?</li>
<li>What are the aims and the approach taken in this textbook?</li>
<li>How is the textbook designed to support attaining these aims?</li>
<li>What is needed to get started?</li>
</ul>
</div>

From time to time there will be points for you to consider and questions to explore. 

<div class="rmdquestion">
<p>Consider the objectives in this course: what ways can the knowledge
and skills you will learn benefit you in your academic studies and/ or
professional and personal life?</p>
</div>

Case studies are provided in-line which highlight key concepts and/ or methodological approaches relevant to the current topic or section.

\BeginKnitrBlock{rmdstudy}<div class="rmdstudy">@Eisenstein2012 track the geographic spread of neologisms from city to city in the United States using Twitter data collected between 6/2009 and 5/2011. They only used tweets with geolocation data and then associated each tweet with a zipcode using the US Census. The most populous metropolitan areas were used. They also used the demographics from these areas to make associations between lexical innovations and demographic attributes. From this analysis they are able to reconstruct a network of linguistic influence. One of the main findings is that demographically-similar cities are more likely to share linguistic influence. At the individual level, there is a strong, potentially stronger role of demographics than geographical location.</div>\EndKnitrBlock{rmdstudy}

<!--
\BeginKnitrBlock{rmdstudy}<div class="rmdstudy">@Bukhari2020 ....</div>\EndKnitrBlock{rmdstudy}
-->

Swirl interactive R programming lessons appear at the beginning of each chapter. The lessons provide a guided environment to experience running code in the R console. The instructions to install the `swirl` package and the textbook lessons can be found on the "[Text as Data Resources](https://lin380.github.io/tadr)" site or directly from [GitHub](https://github.com/lin380/swirl).


<div class="rmdcode">
<p><strong>What</strong>: <a
href="https://github.com/lin380/swirl">Intro to Swirl</a><br />
<strong>How</strong>: In the R Console pane load <code>swirl</code>, run
<code>swirl()</code>, and follow prompts to select the lesson.<br />
<strong>Why</strong>: To familiarize you with navigating, selecting, and
completing swirl lessons.</p>
</div>

At the end of each chapter, a text block will provide readers a cue to explore the applied programming demonstrations called "[Recipes](https://lin380.github.io/tadr/articles/)" on the "[Text as Data Resources](https://lin380.github.io/tadr)" site. Readers may add online annotations using the built-in social annotation tool [hypothes.is](https://web.hypothes.is/education/annotated/research/). *Note: Instructors may opt to [create their own private Hypothes.is annotation group](https://web.hypothes.is/creating-groups/).*

<div class="rmdactivity">
<p><strong>What</strong>: <a
href="https://lin380.github.io/tadr/articles/recipe_1.html">Literate
programming I</a><br />
<strong>How</strong>: Read Recipe 1 and participate in the Hypothes.is
online social annotation.<br />
<strong>Why</strong>: To introduce the concept of Literate Programming
using R, RStudio, and R Markdown.</p>
</div>

Hands-on lab activities to implement and extend programming strategies round out each chapter. These labs are found on [GitHub](https://github.com/lin380?q=lab&type=all&language=&sort=name) and can be downloaded and/ or cloned to any RStudio instance (either your computer or on the web [RStudio Cloud](https://www.rstudio.com/products/cloud/)).

<div class="rmdlab">
<p><strong>What</strong>: <a
href="https://github.com/lin380/lab_1">Literate programming I</a><br />
<strong><em>How</em></strong>: Clone, fork, and complete the steps in
Lab 1.<br />
<strong>Why</strong>: To put literate programming techniques covered in
Recipe 1 into practice. Specifically, you will create and edit an R
Markdown document and render a report in PDF format.</p>
</div>

Tips are used to signal helpful hints that might otherwise be overlooked.

<div class="rmdtip">
<p>During a the course of an exploratory work session, many R objects
are often created to test ideas. At some point inspecting the workspace
becomes difficult due to the number of objects displayed using
<code>ls()</code>.</p>
<p>To remove all objects from the workspace, use
<code>rm(list = ls())</code>.</p>
</div>

Errors will be an inevitable part of learning to code, but some errors can be avoided. The text will used the warning text block to highlight common pitfalls and errors.

<div class="rmdwarning">
<p>Hello world!<br />
This is a warning.</p>
</div>

Although this is not intended to be a in-depth introduction to statistical techniques, mathematical formulas will at times be included in the text. These formulas will appear either inline $1 + 1 = 2$ or as block equations.

\begin{equation}
  \hat{c} = \underset{c \in C} {\mathrm{argmax}} ~\hat{P}(c) \prod_i \hat{P}(w_i|c)
  (\#eq:example-formula)
\end{equation}

Data analysis leans heavily on graphical representations. Figures will appear numbered, as in Figure \@ref(fig:test-fig). 

<div class="figure" style="text-align: center">
<img src="01-course_files/figure-html/test-fig-1.png" alt="Test plot from mtcars dataset" width="90%" />
<p class="caption">(\#fig:test-fig)Test plot from mtcars dataset</p>
</div>

Tables, such as Table \@ref(tab:test-tab) will be numbered separately from figures. 


Table: (\#tab:test-tab)Here is a nice table!

| Sepal.Length| Sepal.Width| Petal.Length| Petal.Width|Species |
|------------:|-----------:|------------:|-----------:|:-------|
|          5.1|         3.5|          1.4|         0.2|setosa  |
|          4.9|         3.0|          1.4|         0.2|setosa  |
|          4.7|         3.2|          1.3|         0.2|setosa  |
|          4.6|         3.1|          1.5|         0.2|setosa  |
|          5.0|         3.6|          1.4|         0.2|setosa  |
|          5.4|         3.9|          1.7|         0.4|setosa  |
|          4.6|         3.4|          1.4|         0.3|setosa  |
|          5.0|         3.4|          1.5|         0.2|setosa  |
|          4.4|         2.9|          1.4|         0.2|setosa  |
|          4.9|         3.1|          1.5|         0.1|setosa  |
|          5.4|         3.7|          1.5|         0.2|setosa  |
|          4.8|         3.4|          1.6|         0.2|setosa  |
|          4.8|         3.0|          1.4|         0.1|setosa  |
|          4.3|         3.0|          1.1|         0.1|setosa  |
|          5.8|         4.0|          1.2|         0.2|setosa  |
|          5.7|         4.4|          1.5|         0.4|setosa  |
|          5.4|         3.9|          1.3|         0.4|setosa  |
|          5.1|         3.5|          1.4|         0.3|setosa  |
|          5.7|         3.8|          1.7|         0.3|setosa  |
|          5.1|         3.8|          1.5|         0.3|setosa  |

<!--
## Resources {-}

This coursebook includes the [Text as Data Resources](https://lin380.github.io/tadr/) accompany website. This site itself includes resources to learn and extend R skills relevant for conducting reproducible text analysis research. [Tutorials](https://lin380.github.io/tadr/tutorials/index.html) are provided which provide video, questions, and interactive coding practice. [Recipes](https://lin380.github.io/tadr/articles/index.html) includes worked demonstrations of targeted aspects of R programming. Each of these resources are coordinated to provide the programming skills necessary for the stages of text analysis covered in the coursebook. 

In addition to the Tutorials and Recipes, students are encouraged to engage with the interactive coding `swirl` activities. In contrast to Tutorials, swirl activities will be performed in an RStudio session in the R console. This provides a more authentic experience for learning to use R. 

-->

## Getting started {-}

Before jumping in to the first chapter of this textbook, it is important to prepare your computing environment and understand how to take advantage of the resources available, both those directly associated with the textbook and indirectly associated. 

### R and RStudio {-}

Programming is the backbone for modern quantitative research. R is a popular programming language with statisticians and was adopted by many other fields in natural and social sciences. It is freely downloadable from [The R Project for Statistical Programming](https://www.r-project.org/) website and is available for [macOS, Linux, and Windows](https://cloud.r-project.org/) operating systems.

While R code can be written and executed in many different environments, [RStudio](https://www.rstudio.com/products/rstudio/) provides a very powerful interface that has been widely adopted by R programmers. RStudio is an IDE (Integrated Development Environment) and serves as a dashboard for working with R --therefore you must download and install R before installing RStudio. You may choose to run RStudio on your own computer ([RStudio Desktop](https://www.rstudio.com/products/rstudio/)) or use RStudio on the web ([RStudio Cloud](https://www.rstudio.com/products/cloud/)). There are advantages to both approaches. Either approach will be compatible with this textbook but if you plan to continue to work with R/RStudio in the future at some point you will most likely want to install the desktop version and maintain your own R and RStudio environment.

For more details to install R and RStudio consult the [RStudio Education](https://education.rstudio.com/learn/beginner/) page.
  
### R packages {-}

Throughout your R programming journey you will take advantage of code created by other R users in the form of packages. A package is a downloadable set of functions and/ or datasets which aim to accomplish a given cohesive set of related tasks. There are official R package repositories such as [CRAN](https://cran.r-project.org/) (Comprehensive R Archive Network) and other packages are available on code-sharing repositories such as [GitHub](https://github.com/).

<div class="rmdquestion">
<p>The Comprehensive R Archive Network (CRAN) includes groupings of
popular packages related to a given applied programming task called <a
href="https://cran.r-project.org/web/views/">Task Views</a>. Explore the
available CRAN Task Views listings. Note the variety of areas (tasks)
that are covered in this listing. Now explore in more detail one of the
following task views which are directly related to topics covered in
this textbook noting the associated packages and their descriptions: (1)
Cluster, (2) MachineLearning, (3) NaturalLanguageProcessing, or (4)
ReproducibleResearch.</p>
</div>

You will download a number of packages at different stages of this textbook, but there is a set of packages that will be key to have from the get go. Once you have access to a working R/ RStudio environment, you can proceed to install the following packages.

Install the following packages from CRAN. 

- `tidyverse`
- `rmarkdown`
- `tinytex`    
- `devtools`
- `usethis`
- `swirl`

You can do this by running the following code in the RStudio Console pane. 

```r
install.packages(c("tidyverse", "rmarkdown", "tinytex", "devtools", "usethis", "swirl")) # install key packages from CRAN
```

Or you can use the RStudio Packages pane and click 'Install' and type the names of the packages.

This textbook includes a support package `tadr` which is available on GitHub ([source code](https://github.com/lin380/tadr)). To install this package from a GitHub repository, you run the following code in the RStudio Console pane: 

```r
devtools::install_github("lin380/tadr") # install the tadr package from GitHub
```

Finally, although not a package we will need to download the interactive R programming lessons for this textbook that will be accessed with the `swirl` package. Download these lessons by running the following code in the RStudio Console pane. 

```r
swirl::install_course_github("lin380", "swirl") # install the swirl lessons for this textbook
```

Later in this Preface and then at the beginning of each subsequent chapter there will be swirl lessons to complete. To load and choose a lesson to start, you will run the following code in the RStudio Console pane. 

```r
library(swirl) # load the swirl package
swirl() # run swirl
```

You will then follow the prompts to select and complete the desired lesson. 

### Git and GitHub {-}

[GitHub](https://github.com/) is a code sharing website. Modern computing is highly collaborative and GitHub is a very popular platform for sharing and collaborating on coding projects. The [lab exercises for this textbook](https://github.com/stars/francojc/lists/labs) are shared on GitHub. To access and complete these exercises you will need to [sign up for a (free) GitHub account](https://github.com/signup?ref_cta=Sign+up&ref_loc=header+logged+out&ref_page=%2F&source=header-home) and then set up the version control software `git` on your computing environment. `git` is the conduit to interfacing GitHub and for many `git` will already be installed on your computer (or cloud computing environment). To verify your installation (or for installation instructions) and to set up your `git` configuration, consult the very useful [Happy Git and GitHub for the useR](https://happygitwithr.com/) chapter [Install Git](https://happygitwithr.com/install-git.html).

### Getting help {-}

The technologies employed in this approach to text analysis will include a somewhat steep learning curve. And in all honesty, the learning never stops! Experienced programmers and novices alike require support. Fortunately there is a very large community of programmers who have developed many official support resources and who actively contribute to unofficial discussion forums. Together these resources provide ample methods for overcoming any challenge.

The easiest and most convenient place to get help with either R or RStudio is through the RStudio "Help" toolbar menu. There you will find links to help resources, guides, and manuals. R packages often include "Vignettes" (long-form documentation and demonstrations). These can be accessed either by running `browseVignettes()` in the RStudio Console pane or by searching for the package using a search engine in your web browser and consulting the package documentation there (e.g. [`usethis`](https://usethis.r-lib.org/)). For some of the more common packages you can find [cheatsheets](https://www.rstudio.com/resources/cheatsheets/) on the RStudio website.

For Git and GitHub I recommend [Happy Git and GitHub for the useR](https://happygitwithr.com/) but the official [Git](https://git-scm.com/doc) and [GitHub](https://docs.github.com/en) documentation pages are great resources as well.

There are a number of very popular discussion forum websites where the programming community asks and answers questions to real-world issues. These sites often have subsections dedicated to particular programming languages or software. Here is a list of some of the most useful in my experience: 

- StackOverflow: [R](https://stackoverflow.com/questions/tagged/r), [Git](https://stackoverflow.com/questions/tagged/git), [RStudio](https://stackoverflow.com/questions/tagged/rstudio), [GitHub](https://stackoverflow.com/questions/tagged/github)
- Reddit: [R](https://www.reddit.com/r/rstats/), [Git](https://www.reddit.com/r/git/), [RStudio](https://www.reddit.com/r/RStudio/), [Github](https://www.reddit.com/r/github/)
- [RStudio Community](https://community.rstudio.com/)

The take-home message here is that you are not alone. There are many people world-wide that are learning to program and/ or contribute to the learning of others. The more you engage with these resources and communities the more successful your learning will be. As soon as you are able, pay it forward. Posting questions and offering answers helps the community and engages and refines your skills --a win-win.

## Activities {-}

<div class="rmdcode">
<p><strong>What</strong>: <a
href="https://github.com/lin380/swirl">Intro to Swirl</a><br />
<strong>How</strong>: In the R Console pane load <code>swirl</code>, run
<code>swirl()</code>, and follow prompts to select the lesson.<br />
<strong>Why</strong>: To familiarize you with navigating, selecting, and
completing swirl lessons.</p>
</div>

<div class="rmdactivity">
<p><strong>What</strong>: <a
href="https://lin380.github.io/tadr/articles/recipe_1.html">Literate
programming I</a><br />
<strong>How</strong>: Read Recipe 1 and participate in the Hypothes.is
online social annotation.<br />
<strong>Why</strong>: To introduce the concept of Literate Programming
using R, RStudio, and R Markdown.</p>
</div>

<div class="rmdlab">
<p><strong>What</strong>: <a
href="https://github.com/lin380/lab_1">Literate programming I</a><br />
<strong>How</strong>: Clone, fork, and complete the steps in Lab
1.<br />
<strong>Why</strong>: To put literate programming techniques covered in
Recipe 1 into practice. Specifically, you will create and edit an R
Markdown document and render a report in PDF format.</p>
</div>

## Summary {-}

In this preface I've provided the rationale and aims of this textbook. The structure of the texbook and the associated resources work to scaffold your learning and proficiency in the areas of Data literacy, Research skills, and Programming skills. The textbook include a series of conventions to signal important concepts, questions to explore, and resources available. As in the area of Data Science in general, quantitative text analysis is most effectively conducted using programmatic approaches. The process will not be without challenges but the gains are well worth the effort. I've outlined key resources to obtain support that are invaluable for the novice as well as the seasoned practitioner. 


