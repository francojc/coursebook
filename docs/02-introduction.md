# (PART) Foundations {-}

# Overview {-#foundations-overview}





**FOUNDATIONS**

<!-- edit -->
In this section the aims are to (1) provide an overview of quantitative research and their applications, by both highlighting visible applications and notable research in various fields. (2) We will under the hood a bit and consider how quantitative research contributes to language research. (3) I will layout the main types of research and situate quantitative text analysis inside these. Some attention will be given to the historical background to understand how theory (generative and usage-based grammar) has framed and to some degree continues to frame language research. (4) We will discuss how the programmatic approaches to language, which are fundamental for quantitative text analysis, also provide the opportunity to further science through process documentation and research reproducibility.  

# Data, language, and text analysis

<p style="font-weight:bold; color:red;">DRAFT</p>

> Science walks forward on two feet, namely theory and experiment...Sometimes it is one foot which is put forward first, sometimes the other, but continuous progress is only made by the use of both.
> ---[Robert A. Millikan](https://www.nobelprize.org/uploads/2018/06/millikan-lecture.pdf) [-@Millikan1923]

<div class="rmdkey">
<p>The essential questions for this chapter are:</p>
<ul>
<li>What is the role and goals of data analysis in and outside of academia?</li>
<li>In what ways is quantitative language research approached?</li>
<li>What are some of the applications of text analysis?</li>
<li>How is this coursebook structured and what are the target learning goals?</li>
</ul>
</div>

<!-- COURSE STRUCTURE
TUTORIALS:

- Git-it: https://github.com/jlord/git-it-electron (interactive app to learn the basics of Git)
- Primers:
  - Programming Basics: https://rstudio.cloud/learn/primers/1.2
  - What is Rmarkdown? https://rmarkdown.rstudio.com/lesson-1.html
  

SWIRL:

- Variables and vectors
- Workspace

WORKED/ RECIPE:

- Literate programming
- GitHub collaboration

PROJECT:

- Interest statement, annotated references, goal(s), finding(s)

-->


<!-- Goals -->

In this chapter I will aim to introduce the topic of text analysis and text analytics and frame the approach of this coursebook. The goals of this section are to work from the general field of data science/ data analysis to the particular sub-field of text analysis (where text is defined broadly as corpus). The aim is to introduce the context needed to understand how text analysis fits in a larger universe of data analysis and see the commonalities in the ever-ubiquitous field of data analysis, with attention to how language and linguistics studies employ data analysis down to the particular area of text analysis. To round out this chapter, I will provide a general overview of the rest of the coursebook motivating the general structure and sequencing as well as setting the foundation for programmatic approaches to data analysis.


## Making sense of a complex world

<!-- Making sense of a complex world 

- world of signals; objects, actions, and interactions
- humans strengths (implicit heuristics) and limitations (perspective, limited storage and limited fidelity) in making sense of the world
- the role of science to address human limitations
  - systematic, rigorous data collection and analysis, reporting
  - collective vetting from scientific community
  - repeat

-->

The world around us is full of actions and interactions so numerous that it is difficult to really comprehend. Through the lens each individual sees and experiences this world. We gain knowledge about this world and build up heuristic knowledge about how it works and how we do and can interact with it. This happens regardless of your educational background. As humans we are built for this. Our minds process countless sensory inputs many of which never make it to our conscious mind. They underlie skills and abilities that we take for granted like being able to predict what will happen if you see someone about to knock a wine glass off a table and onto a concrete floor. You've never seen this object before and this is the first time you've been to this winery, but somehow and from somewhere you 'instinctively' make an effort to warn the would-be-glass-breaker before it is too late. You most likely have not stopped to consider where this predictive knowledge has come from, or if you have, you may have just chalked it up to 'common sense'. As common as it may be, it is an incredible display of the brain's capacity to monitor your environment, relate the events and observations that take place, and store that information all the time not making a big fuss to tell you conscious mind what it's up to. 

So wait, this is a coursebook on text analytics and language, right? So what does all this have to do with that? Well, there are two points to make that are relevant for framing our journey: (1) the world is full of countless information which unfold in real-time at a scale that is daunting and (2) for all the power of the brain that works so efficiently behind the scene making sense of the world, we are one individual living one life that has a limited view of the world at large. Let me expand on these two points a little more. 

First let's be clear. There is no way for any one to experience all things at all times, i.e. omnipotence. But even extremely reduced slices of reality are still vastly outside of our experiental capacity, at least in real-time. One can make the point that since the inception of the internet an individual's ability to experience larger slices of the world has increased. But could you imagine reading, watching, and listening to every file that is currently accessible on the web? (or has been see the Wayback Machine)? Scale this back even further; let's take Wikipedia, the world's largest encyclopedia. Can you imagine reading every wiki entry? As large as a resource such as Wikipedia is ^[ADD: size of Wikipedia], it is still a small fragment of the written language that is produced on the web, just the web. Consider that for a moment.

To my second framing point, which is actually two points in one. I made underscored the efficiency of our brain's capacity to make sense of the world. That efficiency comes from some clever evolutionary twists that lead our brain to take in the world but it makes some shortcuts that compress the raw experience into heuristic understanding. What that means is that the brain is not a supercomputer. It does not store every experience in raw form, we do not have access to the records of our experience like we would imagine a computer would have access to the records logged in a database. Where our brains do excel is in making associations and predictions that help us (most of the time) navigate the complex world we inhabit. This point is key --our brains are doing some amazing work, but that work can give us the impression that we understand the world in more detail that we actually do. Let's do a little thought experiment. Close your eyes and think about the last time you saw your best friend. What were they wearing? Can you remember the colors? If your like me, or any other human, you probably will have a pretty confident feeling that you know the answers to these questions and there is a chance you a right. But it has been demonstrated in numerous experiments on human memory that our confidence does not correlate with accuracy. (where were you when ..? JFK, 9/11, ...other example) You've experienced an event, but there is no real reason that we should be our lives on what we experienced. It's a little bit scary, for sure, but the magic is that it works 'good enough' for practical purposes.

So here's the deal: as humans we are (1) clearly unable to experience large swaths of experience by the simple fact that we are individuals living individual lives and (2) the experiences we do live are not recorded with precision and therefore we cannot 'trust' our intuitions, at least in an absolute sense. 

<!-- Role of science in data analysis -->

What does that mean for our human curiosity about the world around us and our ability to reliably make sense of it? In short it means that we need to approach understanding our world with the tools of science. Science is so powerful because it makes strides to overcome our inherit limitations as humans (breadth of our experience and recall and relational abilities) and bring a complex world into a more digestible perspective. Science starts with question, identifies and collects data, careful selected slices of the complex world, submits this data to analysis through clearly defined and reproducible procedures, and reports the results for others to evaluate. This process is repeated, modifying, and manipulating the procedures, asking new questions and positing new explanations, all in an effort to make inroads to bring the complex into tangible view. 

In essence what science does is attempt to subvert our inherent limitations in understanding by drawing on carefully and purposefully collected slices of experience and letting the analysis of this experience speak, even if it goes against our intuitions (those powerful but sometime spurious heuristics that our brains use to make sense of the world). 

## Data analysis

<!-- The science of data 




-->

At this point I've sketched an outline strengths and limitations of humans' ability to make sense of the world and why science to address these limitations. This science I've described is the one you are familiar with and it has been an indespensible tool to make sense of the world. If you are like me, this description of science may be associated with visions of white coats, labs, and petri dishes. While science's foundation still stands strong in the 21st century, a series of intellectual and technological events mid-20th century set in motion changes that have changed aspects about how science is done, not why it is done. We could call this Science 2.0, but let's use the more popularized term "Data Science". The recognized beginnings of Data Science are attributed to work in the "Statistics and Data Analysis Research" department at Bell Labs during the 1960s. Although primarily conceptual and theoretic at the time, a framework for quantitative data analysis took shape that would anticipate what would come: sizable datasets which would "[...]require advanced statistical and computational techniques [...] and the software to implement them." [@Chambers2020] This framework emphasized both the inference-based research of traditional science, but also embraced exploratory research and recognized the need to address practical considerations that would arise when working with and deriving insight from an abundance of data. 

Fast-forward to the 21st century a world in which machine readable data is truly in abundance. With increased computing power and innovative uses of this technology the world wide web took flight. To put this in perspective, focusing in on language, the amount of text [here add stats on amount of data added to the web every day/month/year compared to all the literature from .. to ..?]. The data flood has not been limited to language, there are more sensors and recording devices than ever before which capture evermore swaths of the world we live in [@Desjardins2019]. Where increased computing power gave rise to the influx of data, it is also on of the primary methods for gathering, preparing, transforming, analyzing, and communicating insight derived from this data [@Donoho2017]. The vision laid out in the 1960s at Bell Labs had come to fruition. 

The interest in deriving insight from the available data is now almost ubiquitous. The science of data has now reached deep into all aspects of life where making sense of the world is sought. Predicting whether a loan applicant will get a loan [cite], whether a lump is cancerous [cite], what films to recommend based on your previous viewing history [cite], what players a sports team should sign [@Lewis2004] all now incorporate a common set of data analysis tools. 

These advances, however, are not predicated on data alone. As envisioned by researchers at Bell Labs, turning data into insight it takes computing skills (i.e. programming), knowledge of statistics, and, importantly, substantive/ domain expertise. This triad has been popularly represented by Drew Conway in a Venn diagram \@ref(fig:intro-data-science-venn). 

<div class="figure" style="text-align: center">
<img src="images/02-introduction/Data_Science_VD.png" alt="[Venn diagram](http://drewconway.com/zia/2013/3/26/the-data-science-venn-diagram) by Drew Conway" width="90%" />
<p class="caption">(\#fig:intro-data-science-venn)[Venn diagram](http://drewconway.com/zia/2013/3/26/the-data-science-venn-diagram) by Drew Conway</p>
</div>

This same toolbelt underlies well-known public-facing language applications. From the language-capable personal assistant applications, plagiarism detection software, machine translation and search, tangible results of quantitative approaches to language are becoming standard fixtures in our lives. 

<!-- Highly visible applications in language -->

<div class="figure" style="text-align: center">
<img src="images/02-introduction/well-known-language-applications.png" alt="Well-known language applications" width="90%" />
<p class="caption">(\#fig:intro-language-applications)Well-known language applications</p>
</div>

The spread of quantitative data analysis too has taken root in academia. Even in areas that on first blush don't appear to be approached in a quantitative manner such as fields in the social sciences and humanities, data science is making important and sometimes disisplinary changes to the way that academic research is conducted. This coursebook focuses in on a domain that cuts across many of these fields; namely language. At this point let's turn to quantitative approaches to language.  


<!-- I want to steer the conversation more towards *the use of science to expand into areas of understanding the world, both in academia and in professional life.* One thought I had today in the gym is to introduce the __Moneyball__ case as an example of how traditional, human-based intuition has it's limitations and how approaching behavior and understanding the underlying mechanisms can be enhanced by scientific approaches. Moneyball is a good first case as it is most likely known by students, but it also is a well-documented case of how traditional wisdom was challenged and loss to rigorous data-driven analysis. -->


<!-- What I need to reconcile is the trajectory of human-based bias, science, and the expanding use of scientific approaches to a wide variety of areas and professions as the availability of data becomes more widespread and computing resources and statistical approaches more robust.  -->

## Language analysis

Language is a defining characteristic of our species. As such, the study of language is of key concern to a wide variety of fields, not just linguists. The goals of various fields, however, and as such approaches to language research, vary. <!-- include a distinction between language form and language as a cultural marker -->On the one hand some language research traditions, namely those closely associated with Noam Chomsky, eschewed quantitative approaches to language research during the later half of the 20th century and instead turned to qualitative assessment of language structure through introspective methods. On the other hand many language research programs turned to and/or developed quantitative research methods either by necessity or through theoretical principles. These quantitative research trajectories share much of the common data analysis toolbox described in the previous section. This means to a large extent language analysis projects share a common research language with other language research but also with research beyond outside of language. However, there is never a one-size-fits all approach to anything --much less data analysis. And in quantitative analysis there is a key distinction in data collection that has downstream effects in terms of procedure but also in terms of interpretation. 

The key distinction, that we need to make at this point, which will provide context for our exploration of text analysis, comes down to the approach to collecting language data and the nature of that data. This distinction is between experimental and observational data collection. Experimental approaches start with a intentionally designed hypothesis and lay out a research methodology with appropriate instruments and a plan to collect data that shows promise for shedding light on the validity of the hypothesis. Experimental approaches are conducted under controlled contexts, usually a lab environment, in which participants are recruited to perform a language related task with stimuli that have been carefully curated by researchers to elicit some aspect of language behavior of interest. Experimental approaches to language research are heavily influenced by procedures adapted from psychology. This link is logical as language is a central area of study in cognitive psychology. This approach looks a much like the white-coat science that we made reference to earlier but, as in most quantitative research, has now taken advantage of the data analysis tool belt to collect and organize much larger quantities of data and conduct statistically more robust analysis procedures and communicate findings more efficiently.

Observational approaches are a bit more of a mixed bag in terms of the rationale for the study; they may either start with a testable hypothesis or in other cases may start with a more open-ended research question to explore. But a more fundamental distinction between the two is drawn in the amount of control the researcher has on contexts and conditions in which the language behavior data to be collected is produced. Observational approaches seek out records of language behavior that is produced by language speakers for communicative purposes in natural(istic) contexts. This may take place in labs (language development, language disorders, etc.), but more often than not, language is collected from sources where speakers are performing language as part of their daily lives --whether that be posting on social media, speaking on the telephone, making political speeches, writing class essays, reporting the latest news for a newspaper, or crafting the next novel destined to be a New York Times best-seller. What is more, data collected from the 'wild' is varies in more in structure relative to data collected in experimental approaches and requires a number of steps to prepare the data to synch up with the data analysis tool belt. 

I liken this distinction between experimental and observational data collection to the difference between farming and foraging. Experimental approaches are like farming; the groundwork for a research plan is designed, much as a field is prepared for seeding, then the researcher performs as series of tasks to produce data, just as a farmer waters and cares for the crops, the results of the process bear fruit, data in our case, and this data is harvested. Observational approaches are like foraging; the researcher scans the available environmental landscape for viable sources of data from all the naturally existing sources, these sources are assessed as to their usefulness and value to address the research question, the most viable is selected, and then the data is collected. 

The data acquired from both of these approaches have their trade-offs, just as farming and foraging. Experimental approaches directly elicit language behavior in highly controlled conditions. This directness and level of control has the benefit of allowing researchers to precisely track how particular experimental conditions effect language behavior. As these conditions are an explicit part of the design and therefore the resulting language behavior can be more precisely attributed to the experimental manipulation. The primary shortcoming of experimental approaches is that there is a level of artificialness to this directness and control. Whether it is the language materials used in the task, the task itself, or the fact that the procedure takes place under supervision the language behavior elicited can diverge quite significantly from language behavior performed in natural communicative settings. Observational approaches show complementary strengths and shortcomings. Whereas experimental approaches may diverge from natural language use, observational approaches strive to identify and collected language behavior data in natural, uncontrolled, and unmonitored contexts. In this way observational approaches do not have to question to what extent the language behavior data is or is not performed as a natural communicative act. On the flipside, the contexts in which natural language communication take place are complex relative to experimental contexts. Language collected from natural contexts are nested within the complex workings of a complex world and as such inevitably include a host of factors and conditions which can prove challenging to disentangle from the language phenomenon of interest but must be addressed in order to draw reliable associations and conclusions. 

The upshot, then, is twofold: (1) data collection methods matter for research design and interpretation and (2) there is no single best approach to data collection, each have their strengths and shortcomings. In the ideal, a robust science of language will include insight from both experimental and observational approaches [@Gilquin:2009]. And evermore there is greater appreciation for the complementary nature of experimental and observational approaches and a growing body of research which highlights this recognition. Given their particular trade-offs observational data is often used as an exploratory starting point to help build insight and form predictions that can then be submitted to experimental conditions. In this way studies based on observational data serve as an exploratory tool to gather a better and more externally valid view of language use which can then serve to make prediction that can be explore with more precision in an experimental paradigm. However, this is not always the case. Observational data is also often used in hypothesis-testing contexts as well. And furthermore, some in some language-related fields, a hypothesis-testing is not the ultimate goal for deriving knowledge and insight. 


<!-- is language research is not  them as In some cases, however, the choice between which data collection method is best suited for a research project will clear. Sometimes experimental data collection is not an option or on the other hand observational data cannot address particular nuances in language behavior.  -->




<!-- I want to bring language into focus. Introducing __empirical approaches to language study__. This discussion should highlight the distinction between experimental data and observational data. -->

<!-- I want to contrast the types and trade-offs associated with both approaches. 

Experimental data is controlled rigorously, recruiting participants, controlling the conditions in which language is presented and behavior is measured. 

Observational data, one the other hand, is not controlled to the same degree. The data is collected in a way in which language is performed in more natural contexts. 

Both approaches have advantages and disadvantages. I want to highlight that although this coursebook focuses on observational data, robust understanding of language behavior requires a collaboration between both approaches.  -->


<!-- I occurs to me that I could try to work out tangible examples of *experimental data and observational data*. The first that comes to mind is observational --the Unibomber manifesto was not a controlled experiment. Language was produced and the FBI had the goal of analyzing the language found within to understand and identify the author (authorship attribution).  -->




## Text analysis


<!-- The __Unibomber manifesto__ brings language into the mix and, again, highlights the inability of individuals to readily detect patterns (the signal) found within texts. The aspect I have in mind is the phrase "Have your cake and eat it to" vs. "Eat your cake and have it to". The FBI was able to build a case against Ted Kasinzki base on this phrase tracing this idiomatic variance to a particular usage which had fallen out of popular usage. -->

<!-- At this point in the chapter I have outlined a number of key concepts that have led us to the main focus of this coursebook: text analysis. I first started by highlighting the fact that humans are both curious animals and that our own in-built capacities, while functionality amazing, are limited in providing insight into the workings of the complex world that we inhabit. The tools of science have served and continue serve to stem these limitations. Emerging technologies have provide the average researcher access to more and more data which in turn requires both computing resources and knowledge and evermore advanced statistical procedures to handle and analyze this data --Data Science in a nutshell. I then highlighted the inroads that quantitative data analysis has made in industry and academics, including language-based and linguistic-centered applications and research. ... -->

Text analysis is the application of data analysis procedures from data science to derive insight from textual data collected through observational methods. I have deliberately chosen the term 'text analysis' to avoid what I see are the pitfalls of using some other common terms in the literature such as Corpus Linguistics, Computational Linguistics, or Digital Humanities. There are plenty of learning resources that focus specifically on one of these three fields when discussing the quantitative analysis of text. But from my perspective what is missing is a resource which underscores the fact that text analysis research and the methods employed span across a wide variety of academic fields and applications in industry. This coursebook aims to introduce you to these areas through the lens of the data and analysis procedures and not from the field. This approach, I hope, provides a wider view of the potential applications of using text as data and inspires you to either employ quantitative text analysis in your research or to raise your awareness of the advantages of text analysis for making sense of language-related and linguistic-based phenomenon.

So what are some applications of text analysis? For most the public facing applications that stem from Computational Linguistic research, often known as Natural Language Processing by practioners, are the most well-known applications of text analysis. Whether it be using search engines, online translators, submitting your paper to plagarism detection software, etc. the text analysis methods we will cover are at play. These uses of text analysis are production-level applications and there is big money behind developing evermore robust text analysis methods. 

In academia the use of text analysis is even more widespread, despite the lack of public fanfare. Let's run through some select studies to give you an idea of the areas that are employing text analysis, of what researchers are doing with text analysis, and to whet your interest for conducting your own text analysis project. 

<!-- language variation and change --> 

\BeginKnitrBlock{rmdtodo}<div class="rmdtodo">@Eisenstein2012 track the geographic spread of neologisms from city to city in the United States using Twitter data collected between 6/2009 and 5/2011. They only used tweets with geolocation data and then associated each tweet with a zipcode using the US Census. The most populous metropolitan areas were used. They also used the demographics from these areas to make associations between lexical innovations and demographic attributes. From this analysis they are able to reconstruct a network of linguistic influence. One of the main findings is that demographically-similar cities are more likely to share linguistic influence. At the individual level, there is a strong, potentially stronger role of demographics than geographical location.</div>\EndKnitrBlock{rmdtodo}

<!-- sociolinguistics -->

\BeginKnitrBlock{rmdtodo}<div class="rmdtodo">@Voigt2017 explore potential racial disparities in officer respect in police body camera footage. The dataset is based on body camera footage from the Oakland Police Department during April 2014. At total of 981 stops by 245 different officers were included (black 682, white 299) and resulted in 36,738 officer utterances. The authors found evidence for racial disparities in respect but not formality of utterances, with less respectful language used with the black community members.</div>\EndKnitrBlock{rmdtodo}

<!-- political science -->

\BeginKnitrBlock{rmdtodo}<div class="rmdtodo">@Conway2012 investigate whether the established drop in language complexity of rhetoric in election seasons is associated with election outcomes. The authors used US Democratic Primary Debates from 2004. The results suggest that although there was no overall difference in complexity between winners and losers, their pattern differed over time. Winners tended to drop the complexity of their language closer to the upcoming election.</div>\EndKnitrBlock{rmdtodo}

<!-- psychology -->

\BeginKnitrBlock{rmdtodo}<div class="rmdtodo">@Kloumann2012 explore the extent to which languages are positively, neutrally, or negatively biased. Using Twitter, Google Books (1520-2008), NY Times newspaper (1987-2007), and music lyrics (1960-2007) the authors extract the top 5,000 most frequent words from each source and have participants rate each word for happiness (9-point scale). The results show that positive words strongly outnumber negative words overall suggesting English is positive-, and pro-social- biased.</div>\EndKnitrBlock{rmdtodo}

<!-- L2 academic writing -->

\BeginKnitrBlock{rmdtodo}<div class="rmdtodo">@Bychkovska2017 investigates possible differences between L1-English and L1-Chinese undergraduate students’ use of lexical bundles, multiword sequences which are extended collocations (i.e. as the result of), in argumentative essays. The authors used the Michigan Corpus of Upper-Level Student Papers (MICUSP) corpus using the argumentative essay section for L1-English and the Corpus of Ohio Learner and Teacher English (COLTE) for the L1-Chinese English essays. They found that L1-Chinese writers used more than 2 times as many bundle types than L1-English peers which they attribute to L1-Chinese writers attempt to avoid uncommon expressions and/or due to their lack of register awareness (conversation has more bundles than writing generally).</div>\EndKnitrBlock{rmdtodo}

<!-- psycholinguistics -->

\BeginKnitrBlock{rmdtodo}<div class="rmdtodo">@Jaeger:2007a use a corpus study to investigate the phenomenon of syntactic persistence, the increased tendency for speakers to use a particular syntactic form over an alternate when the syntactic form is recently processed. The authors attempt to distinguish between two competing explanations for the phenomenon: (1) transient activation, where the increased tendency is short-lived and time-bound and (2) implicit learning, where the increased tendency is a reflect of learning mechanisms. The use of a speech corpora (Switchboard and spoken BNC) were used to avoid the artificialness that typically occurs in experimental settings. The authors investigated the ditransitive alternation (NP PP/ NP NP), voice alternation (active/ passive), and complementizer/ relativizer omission. In these alternations structural bias was established by measuring the probability for a verb form to appear in one of the two syntactic forms. Then the probability that that form (target) would change given previous exposure to the alternative form (prime) was calculated; what the authors called surprisal. Distance between the prime structure and the target verb were considered in the analysis. In these alternations, the less common structure was used in the target more often when the when it corresponded to the prime form (higher surprisal) suggesting that implicit learning underlies syntactic persistence effects.</div>\EndKnitrBlock{rmdtodo}

<!-- language variation/ dialectology -->

\BeginKnitrBlock{rmdtodo}<div class="rmdtodo">@Wulff2007 explore differences between British and American English at the lexico-syntactic level in the *into*-causative construction (ex. ‘He tricked me into employing him.’). The analysis uses newspaper text (The Guardian and LA Times) and the findings suggest that American English uses this construction in verbal persuasion verbs whereas British English uses physical force verbs.</div>\EndKnitrBlock{rmdtodo}

<!-- authorship attribution -->

\BeginKnitrBlock{rmdtodo}<div class="rmdtodo">@Mosteller1963 provide a method for solving the authorship debate surrounding The Federalist papers ^[https://guides.loc.gov/federalist-papers/full-text]. They employ a probabilistic approach using the word frequency profiles of the articles with known authors to predict authorship of the disputed 12 papers. The results suggest that the disputed papers were most likely authored by Madison.</div>\EndKnitrBlock{rmdtodo}

<!-- translation studies -->

\BeginKnitrBlock{rmdtodo}<div class="rmdtodo">@Olohan2008 investigate the extent to which translated texts differ from native texts. In particular the author explores the notion of explicitation in translated texts (the tendency to make information in the source text explicit in the target translation). The study makes use of  the Translational English Corpus (TEC) for translation samples and comparable sections of the British National Corpus (BNC) for the native samples. The results suggest that there is a tendency for syntactic explicitation in the translational corpus (TEC) which is assumed to be a subconscious process employed unwittingly by translators.</div>\EndKnitrBlock{rmdtodo}

This sample of studies include research from areas such as translation, stylistics, language variation, dialectology, psychology, psycholinguistics, political science, and sociolinguistics which highlights the diversity of fields and subareas which employ quantitative text analysis. Text analysis is at the center of these studies as they share a set of common goals: 

1. To detect and retrieve patterns from text too subtle or too numerous to be done by hand
2. To challenge assumptions and/or provide other views from textual sources
3. To explore new questions and/or provide novel insight

Let's now turn to the last section of this chapter which will provide an overview of the rationale for doing learning to do text analysis, the structure of the content covered, and a justification for the approach we will take to perform text analysis. 

## Coursebook overview

<!-- 

In this section I will provide an overview of the coursebook. Specifically I will outline why the student should care about what we will cover (learning outcomes), what we will cover in terms of data literacy (data to insight hierarchy), research skills (research blueprint), and implementation abilities, and how we will will approach text analysis, focusing on the importance of programming skills (R in particular) to create reproducible workflows which enhance their ability to organize and conduct efficient research but also make valuable long-lasting contributions to the field.

-->

In this section I will provide a general overview of the rest of the coursebook motivating the general structure and sequencing as well as setting the foundation for programmatic approaches to data analysis. Let me highlight why I think this is a valuable area of study, what I hope you gain from this coursebook, and how the structure of this coursebook is configured to help scaffold your conceptual and practical knowledge of text analysis. 

<!-- learning outcomes -->

The target learning outcomes in this coursebook are the following:

1. Data Literacy
2. Research Skills
3. Programming Skills

__Data Literacy__ refers to the ability to interpret, assess, and contextualize findings based on data. Throughout this coursebook we will explore topics which will help you understand how data analysis methods derive insight from data. In this process you will be encouraged to critically evaluate connections across linguistic and language-related disciplines using data analysis knowledge and skills. Data Literacy is an invaluable skillset for academics and professionals (cite) but also is an indispensable aptitude for in the 21st century citizens to navigate and actively participate in the 'Information Age' in which we live [@Carmi2020].

__Research skills__ covers the ability to conduct original research, communicate findings, and make meaningful connections with findings in the literature of the field. This target area does not differ significantly, in spirit, from common learning outcomes in a research methods course: identify an area of investigation, develop a viable research question or hypothesis, collect relevant data, analyze data with relevant statistical methods, and interpret and communicate findings. However, working with text will incur a series of key steps in the selection, collection, and preparation of the data that are unique to text analysis projects. In addition, I will stress the importance of research documentation and creating reproducible research as an integral part of modern scientific inquiry. 

__Programming skills__ aims to develop your ability to implement research skills programmatically and produce research that is replicable and collaborative. Modern data analysis, and by extension, text analysis is conducted using programming. There are various key reasons for this: (1) programming affords researchers unlimited research freedom --if you can envision it, you can program it. The same cannot be said for off-the-shelf software which is either proprietary or unmaintained --or both. (2) programming underlies well-documented and reproducible research --documenting button clicks and menu option selections leads to research which is not readily reproduced, either by some other researcher or by your future self! (3) programming forces researchers to engage more intimately with the data and the methods for analysis. The more familiar you are with the data and the methods the more likely you are to produce higher quality work.


<!--  structure, and how it is linked to the learning outcomes -->

Now let me turn to how these learning goals integrate and shape the structure and sequencing of the following chapters. 

In Part II "Orientation" we will build our Data Literacy skills working from data to insight. This progression is visualized in Figure \@ref(fig:diki-hierarchy) ^[Adapted from @Ackoff1989]. 


<div class="figure" style="text-align: center">
<img src="images/02-introduction/diki-hierarchy-updated.png" alt="Data to Insight Hierarchy (DIKI)" width="90%" />
<p class="caption">(\#fig:diki-hierarchy)Data to Insight Hierarchy (DIKI)</p>
</div>

The DIKI Hierarchy highlights the stages and intermediate steps required to derive insight from data. Chapter 2 "Understanding data" will cover both Data and Information covering the conceptual topics of populations versus samples and how language data samples are converted to information and the forms that they can take. In Chapter 3 "Statistical approaches" I will discuss the distinction between descriptive and analytic statistics. In brief they are important for data analysis, but descriptive statistics serve as a sanity check on the dataset before submitting it to interrogation --which is the goal of analytic statistics. We will also cover some of the main distinctions between analytics approaches including inference-, exploration-, and prediction-based methods. With a fundamental understanding of data, information, and knowledge we will then move to Chapter 4 "Framing research" where we will discuss how to develop a research plan, or what I will call a 'research blueprint'. At this point we will directly address Research Skills and elaborate on how research really comes together; how to bring yourself up to speed with the literature on a topic, how to develop a research goal or hypothesis, how to select data which is viable to address the research goal or hypothesis, how to determine the necessary information and appropriate measures to prepare for analysis, how to perform diagnostic statistics on the data and make adjustments before analysis, how to select and perform the relevant analytic statistics given the research goals, how to report your findings, and finally, how to structure your project so that it is well-documented and reproducible. 

Part III "Preparation" and Part IV "Modeling" serve as practical and more detailed guides to the R programming strategies to conduct text analysis research and as such develop your Programming Skills. In Chapter 5 "Acquire data" I will discuss three main strategies for accessing data: direct downloads, Automatic Programming Interfaces (APIs), and web scraping. In Chapter 6 "Curate data" I will outline the process for converting or augmenting the acquired data into a structured format, therefore creating information. This will include organizing linguistic and non-linguistic metadata into one dataset. In Chapter 7 "Transform data" I describe how to work with a curated dataset to derive more detailed information and appropriate dataset structures that are appropriate for the upcoming analysis. 

Chapters 8 "Exploration", 9 "Inference", and 10 "Prediction" focus on different categories of statistical analysis each associated with distinct research goals. Exploration covers 'bottom-up'-style, or 'unsupervised learning', analysis methods such as association measures, clustering, topic modeling, and vector-space models. These methods are aligned with research goals that aim to interpret patterns that arise in from the data itself. Inference deals with analysis methods associated with standard hypothesis-testing. This will include some common statistical models employed in text analysis: chi-squared, logistic regression, and linear regression. Prediction explores a set of statistical methods known as 'supervised learning'. Similar to unsupervised learning, prediction models are employed in a bottom-up fashion. However, the key distinction is that the dataset includes an organizing 'class' variable which the statistical methods aim to model in order to formulate a generalization that can correctly classify new textual data. I will cover some standard methods for text classification including Näive Bayes, *k*-nearest neighbors (*k*-NN), and decisions tree and random forest models. 

## Summary

In this chapter I started with some general observations about the difficulty of making sense of a complex world. The standard approach to overcoming inherent human limitations in sense making is science. In the 21st century the toolbelt for doing scientific research and exploration has grown in terms of the amount of data available, the statistical methods for analyzing the data, and the computational power to manage, store, and share the data, methods, and results from quantitative research. The methods and tools for deriving insight from data have made significant inroads in and outside academia, and increasingly figure in the quantitative investigation of language. Text analysis is a particular branch of this enterprise based on observational data from real-world language and is used in a wide variety of fields. This coursebook aims to develop your knowledge and skills in three fundamental areas: Data Literacy, Research Skills, and Programming Skills.

In the end I hope that you enjoy this exploration into text analysis. Although learning curve at times may seem steep --the experience you will gain will not only improve your data literacy, research skills, and programmings skills but also enhance your appreciation for the richness of human language and its important role in our everyday lives.


<!-- Programming with R

- add advantages and shortcomings to programming and
- advantages and alternatives to R 

in the preface (01-course.Rmd) document.

-->



<!---

## Annotated readings

### Data analysis

**Lewis, Michael. 2004. Moneyball: The Art of Winning an Unfair Game. WW Norton & Company.** [@Lewis2004]

This is the story of the Oakland A's baseball team and the use of data analytics to maximize the use of their salary cap to acquire the most useful players based on metrics that were overlooked previously.

It is a story in how applied data science can uncover patterns that tend to be overlooked or are not visible without a scientific inquiry and the use of practical data science to find patterns. (p. 50)

**Chambers, J. M. (2020). S, R, and data science. Proceedings of the ACM on Programming Languages, 4(HOPL), 1–17. https://doi.org/10.1145/3386334** [@Chambers2020]


A definition of Data Science: "Data science consists of techniques and their application to derive and communicate scientifically valid inferences and predictions based on relevant data." (p. 2)

"Data analysis as practiced at Bell Labs is recognized as the precursor of what would now be described as 'data science'". (p. 1)

Work at Bell Labs consisted of what now is considered typical practices in data science "large datasets; iterative, probing analysis including visualization; problems of practical importance and, as a result, challenging computations. Data analysis that was useful and applicable to sizable datasets required advanced computational techniques for the time and good software to implement them."

That is, the practice required advanced statistical and computational techniques --these are the characteristics that distinguish 'data science' and other forms of traditional scientific research. 


```r
knitr::include_graphics("images/02-introduction/ngram-viewer-data.png")
```

<div class="figure" style="text-align: center">
<img src="images/02-introduction/ngram-viewer-data.png" alt="Google Ngram Viewer" width="100%" />
<p class="caption">(\#fig:ngram-viewer-data)Google Ngram Viewer</p>
</div>

Data science, and related terms, are in large part applied statistics. But there is much more that falls under the umbrella which falls outside of what one would consider statistics proper (see @Donoho2017).


**Donoho, D. (2017). 50 Years of Data Science. Journal of Computational and Graphical Statistics, 26(4), 745–766. https://doi.org/10.1080/10618600.2017.1384734** [@Donoho2017]

The author suggests what is coined "Data Science" is really six sub-divisions: 

1. Data Gathering, Preparation, and Exploration 
2. Data Representation and Transformation
3. Computing with Data
4. Data Modeling
5. Data Visualization and Presentation 
6. Science about Data Science

**Gupta, A. (2020, August 19). Data, Information, Knowledge, and Insights. https://www.linkedin.com/pulse/data-information-knowledge-insights-achin-gupta** [@Gupta2020]


```r
knitr::include_graphics("images/02-introduction/dikw-conspiracy.jpg")
```

<img src="images/02-introduction/dikw-conspiracy.jpg" width="90%" style="display: block; margin: auto;" />
**Chen, M., Ebert, D., Hagen, H., Laramee, R. S., Van Liere, R., Ma, K.-L., Ribarsky, W., Scheuermann, G., & Silver, D. (2008). Data, information, and knowledge in visualization. IEEE Computer Graphics and Applications, 29(1), 12–19.** [@Chen2008]

> __Data__: a representation of facts, concepts, or instructions in a formalized manner suitable for communication, interpretation, or processing by human beings or by automatic means.

> __Information__: the meaning that is currently assigned [by human beings or computers] to data by means of the conventions applied to those data. 

> __Knowledge__: understanding, awareness, or familiarity acquired through education or experience. Anything that has been learned, perceived, discovered, inferred, or understood.

"Despite the lack of an agreeable set of the definitions of data, information, and knowledge, a consensus exists that data isn't information and that information isn't knowledge."

**Ackoff, R. L. (1989). From data to wisdom. Journal of Applied Systems Analysis, 16(1), 3–9.** [@Ackoff1989]

- Data are symbols that represent the properties of objects and events. 
- Information consists of processed data, the processing directed at increasing its usefulness. 
- Knowledge is conveyed by instructions, answers to how-to questions.
- Understanding (Insight) is conveyed by explanations, answers to why questions.

From all this I infer that although we are able to develop computerized information-, knowledge-, and understanding-generating systems, we will never be able to generate wisdom by such systems. It may well be that wisdom—which is essential for the pursuit of ideals or ultimately valued ends—is the characteristic that differentiates man from machines. 

**Rowley, J. (2007). The wisdom hierarchy: Representations of the DIKW hierarchy. Journal of Information Science, 33(2), 163–180. https://doi.org/10.1177/0165551506070706** [@Rowley2007]


```r
knitr::include_graphics("images/02-introduction/Rowley-dikw.png")
```

<div class="figure" style="text-align: center">
<img src="images/02-introduction/Rowley-dikw.png" alt="The wisdom hierarchy, Rowley(2007)" width="90%" />
<p class="caption">(\#fig:dikw-rowley)The wisdom hierarchy, Rowley(2007)</p>
</div>


### Language analysis

**Levshina, N. (2015). How to do linguistics with R: Data exploration and statistical analysis. John Benjamins Publishing Company.** [@Levshina2015]

Chapter 2 "The quantitative turn in Linguistics" 

- Notes the gain in popularity of quantitative language research. Usage-based approaches, Cognitive Linguistics, Variationist approaches, etc. 

- Stresses the importance of using multivariate methods for studying and understanding the complexities of language.

- Also makes point that multiple kinds of evidence are key to understanding language behavior. 

### Text analysis


### Goals and organization

__Goals__

- Data Literacy (DL) - ability to interpret, assess, and contextualize findings based on data
- Information Literacy (IL) - ability to locate, evaluate, and use effectively the needed information
- Statistical Literacy (SL) - ability to use statistics as evidence in arguments
- Research Skills (RS) - ability to conduct original research, communicate findings, and make meaningful connections with the field
- Programming Skills (PS) - ability to implement research skills in a replicable form

__Why__

- ...


__What__

- Data to Insight

My modified DIKW to DIKI:


```r
knitr::include_graphics("images/02-introduction/diki-hierarchy.png")
```

<img src="images/02-introduction/diki-hierarchy.png" width="90%" style="display: block; margin: auto;" />

NOTE: I would modify Insight to "Contributions" and "Connections". I leave off wisdom as it is the last extension which deals with "effectiveness" and ultimately is judgment-level knowledge.


- Research blueprint

- Preparation

- Modeling

__How__

- Programming

-->





