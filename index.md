## Objectives

Human culture provides an ideal testbed for students exploring data science. It's a challenging space to work in, because most cultural materials start out as unstructured texts, sound files, or images--not neat spreadsheets. Humanistic questions also highlight the importance of interpreting statistical models in relation to a social context. Last but not least: songs, poems, and stories confront us with vivid problems that are inherently fun to explore.

Our main goals in the course are to

- understand what kinds of insights data science can (and can't) provide about human culture
- get hands-on experience using Python to model texts and images
- understand the mathematical principles underlying statistical machine learning, including a glimpse of deep learning

## Assignments 

There are three kinds of assignments in this class: homework (in Python), informal posts in the discussion forum, and a final project (individual or group) that uses data science to investigate a question about history or human culture.

**Homework.** There will be ten homework assignments. Each one takes the form of a Jupyter notebook. In the early weeks of the class I will usually start the notebook and then ask you to finish it in a way that addresses a short list of questions.

You might consider creating a subfolder within is417 named with your netID (e.g. for me it would be ```tunder/```), and keeping your homework assignments (just the ```.ipynb``` files) in that folder. At a later stage of the semester, this might make it easier to share your homework with me using git so I can help you debug it. However, for now I don't recommend using git to submit homework. Instead, print your notebook as a .pdf file (you can do this under "File" in JupyterLab) and submit the .pdf on the Moodle, with the .ipynb file as an attachment.

I will drop the lowest homework grade, so if you miss one, that's not a disaster.

**Forum posts.** Five times during the semester, write a brief paragraph-length comment in the discussion forum. Usually these will be comments on the reading for a particular day; I'll use them to organize discussion. Toward the end of the class we'll be using the forum to discuss challenges you've encountered in your projects.

**Final project.** Write an 8-12 page paper that uses some form of quantitative analysis to illuminate a question about human history or contemporary culture. Your results don't necessarily have to take the form of an experimental report (data-methods-results-conclusions). Some projects might more appropriately produce an annotated map, for instance, accompanied by a narrative. We're in a space between disciplines, so form is a place where you can be creative. 

Please don't feel that your project has to demonstrate advanced methods. We're going to explore recent advanced topics here, but complex methods are not useful for all problems. Sometimes all you need is manual counting ("How many people does John Wick shoot?") plus a simple calculation ("compare to the median body count in other films").

These can be individual projects or group work. If you decide to organize in a group, you can be a more ambitious in your data gathering and analysis, and perhaps produce a slightly longer (10-16 page) paper.

Papers should be supported by code and data showing how you reached your conclusion. If you would like to make your project visible to an audience beyond the class, one way to organize your expository report, code, and data is to create a GitHub repository, like the one you're reading now.

Homework assignments are worth 60% of the grade, forum posts and synchronous participation are worth 10%, and your final project is worth 30%.

![The Wisdom of the Ancients](https://imgs.xkcd.com/comics/wisdom_of_the_ancients.png)

### Getting help on assignments

I like Miriam Posner's ["ground rules for learning tech,"](https://twitter.com/miriamkp/status/1349095892700205057) and aspire to imitate them here.

In particular, I want to stress that I don't see the homework assignments as "tests." My goal is for everyone to succeed on all the assignments. 

Always start by trying to solve the problem yourself. A big part of learning to code is learning to make (and catch) mistakes, and that involves a certain amount of staring at the screen, googling whatever error message you're getting, [cursing DenverCoder9](https://xkcd.com/979/), groaning, etc. But if you've done that for an hour straight and seem to be hitting the same wall over and over, it's time to get help. Often it's something very simple! You can email me, or another student in class, and ask for a tip. Let me underline that again, because these ground rules are different from some classes: *I'm saying it's fine to email another student and ask for a clue*. The final notebook should be your own work, but it's okay to ask for help. (Don't post solutions openly on the class forum, though, because it's really important for people to google the error message and curse DenverCoder9 first. Someday you'll hit a problem where no one knows the answer yet, and then it's going to matter that you've had a lot of practice groaning, enduring, trying different debugging strategies, etc.) 

Do acknowledge help in the notebook. "I copied parts of the sort_lyrics() function from DenverCoder9 at Stack Overflow, and also got advice from my roommate Carol." This will not detract from your grade; it's normal to borrow bits of code.

If you email me for help, I will try to respond within 48 hours, but I need to warn you in advance that a 48- to 72-hour delay is typical.

### Where I got help

This syllabus is strongly influenced by (and sometimes borrows directly from) two recent courses: Melanie Walsh, ["Introduction to Cultural Analytics and Python,"](https://melaniewalsh.github.io/Intro-Cultural-Analytics/features/Data-Analysis/Pandas-Basics-Part1.html) as well as Dan Sinykin, ["Practical Approaches to Data Science with Text."](https://github.com/sinykin/QTM-340/blob/master/docs/schedule.md)

# Schedule

Note that homework stops after March, and reading really slows down too, so you can focus on your projects.

### January 25: Introduction to Jupyter and Python

**What are the humanities?**
[Familiar answers, from 4Humanities.]
(https://4humanities.org/2014/12/what-are-the-humanities/)

[Puzzling evidence from the Google ngram viewer.]
(https://rb.gy/1rbtj2)

**What happens when the humanities meet data science?**
Mohr, Wagner-Pacifici, and Breiger, ["Toward a Computational Hermeneutics."](https://journals.sagepub.com/doi/full/10.1177/2053951715613809)

We'll discuss this article in some depth.

Campo-Rembado and Oakley, ["How 20th Century Fox Uses ML to Predict a Movie Audience."](https://cloud.google.com/blog/products/ai-machine-learning/how-20th-century-fox-uses-ml-to-predict-a-movie-audience)

Don't worry deeply about the technical details here; I'm not planning to discuss this piece in depth--just giving you a glimpse of what's possible.

**Lab session:**

Walsh, ["The Command Line"](https://melaniewalsh.github.io/Intro-Cultural-Analytics/features/Command-Line/The-Command-Line.html) and ["How To Use Jupyter Notebooks"](https://melaniewalsh.github.io/Intro-Cultural-Analytics/features/Python/How-to-Use-Jupyter-Notebooks.html) are useful preparation.

Install git and clone the IS417 repository. This will give you
[```Milne_ALostMasterpiece.txt```](https://americanliterature.com/author/aa-milne/essay/a-lost-masterpiece) in the ```texts/``` directory, and
```simple_word_counting.ipynb``` in the ```labs/``` subdirectory.

See if you can run ```simple_word_counting.ipynb.```

**Homework 1:** Write code blocks that
a) check whether a word contains any repeated letters,
b) test whether two words are anagrams,
c) (optional, not required, just for fun) find all common English words that are anagrams for a given string.

If you don't have previous experience with Python, you may want to work through [sections 2-7 of "The Python Tutorial"](https://docs.python.org/3/tutorial/) before attempting the homework. Other introductory books and online tutorials could work equally well; Melanie Walsh has good chapters on Lists, Loops, String Methods, and Dictionaries that can be downloaded as notebooks.

### Warning: everything after this is tentative and will definitely get revised!

### February 1: Descriptive and Inferential Statistics with Pandas

Anelise Hanson Shrout, ["(Re)Humanizing Data: Digitally Navigating the Bellevue Almshouse."](https://crdh.rrchnm.org/essays/v01-10-(re)-humanizing-data/)
Melanie Walsh, ["Pandas Basics."](https://melaniewalsh.github.io/Intro-Cultural-Analytics/features/Data-Analysis/Pandas-Basics-Part1.html)

Before class, work through the notebook ```MoviesAndStatistics.ipynb.```

David Robinson, ["Text Analysis of Trump's Tweets Confirms He Writes Only the (Angrier) Android Half."](http://varianceexplained.org/r/trump-tweets/)

Benjamin Schmidt, ["Comparing Corpuses by Word Use."](http://sappingattention.blogspot.com/2011/10/comparing-corpuses-by-word-use.html)

optional background: Ted Dunning, ["Accurate Methods for the Statistics of Surprise and Coincidence."](https://www.aclweb.org/anthology/J93-1003.pdf)

**Lab session:**

Can we improve on Robinson's analysis, and find words that are significantly over-represented in the Android tweets?

**Homework 2:**

Questions about movie dialogue, by period, genre, and character gender.

If you need more background on descriptive and inferential statistics, I recommend the free [*OpenIntro Statistics.*](https://leanpub.com/openintro-statistics)


### February 8: Probability and statistical learning
Daniel Jurafsky and James H. Martin, [Section 3.1, "Ngrams"](https://web.stanford.edu/~jurafsky/slp3/3.pdf)

For intuition, Stephanie Yee and Tony Chu, [“A Visual Introduction to Machine Learning.”](http://www.r2d3.us/visual-intro-to-machine-learning-part-1/) You may also enjoy ["Part 2: Model Tuning and the Bias-Variance Tradeoff."](http://www.r2d3.us/visual-intro-to-machine-learning-part-2/)

Daniel Jurafsky and James H. Martin, [all of Chapter 4, "Naive Bayes and Sentiment Classification."](https://web.stanford.edu/~jurafsky/slp3/4.pdf)

**Lab session:**

We'll build a Naive Bayes classifier and model the sentiment of movie reviews.

**Homework 3**

### February 15: High-Dimensional Space: Where the Humanities Happen

Daniel Jurafsky and James H. Martin, "Vector Semantics & Embeddings": Sections 6-6.4

Victor Powell, [“Principal component analysis explained visually.”](https://setosa.io/ev/principal-component-analysis/)

Alison et al., “Quantitative Formalism.”

Before class, work through the notebook ```MovieSimilarity.ipynb```

Optional: Matt Daniels, ["The Language of Hip Hop."](https://pudding.cool/2017/09/hip-hop-words/)

**Lab session**:

We'll perform principal component analysis on movies, and measure the similarity of words in "dialogue space."

**Homework 4:**

Principal component analysis on movie genres.

### February 22: How to Learn in High-Dimensional Space: Logistic Regression

James, Witten, Hastie, and Tibshirani, "2. Statistical Learning," "4. Classification," and "5.1 Cross-Validation" from *An Introduction to Statistical Learning.*

As you read these chapters, work through the paired notebook ```HumanitiesML.ipynb," which will show you how to apply the principles explained in James et al. using Python rather than the R they use.

Vincent Spruyt, ["The Curse of Dimensionality in Classification."](https://www.visiondummy.com/2014/04/curse-dimensionality-affect-classification/)

**Lab session**

We'll measure the strength of gender stereotypes in movie dialogue.

**Homework 5:**

Do gender stereotypes change across time?


### March 1: Topic Modeling

**Homework 6**

### March 8: Beyond Bags of Words: People, Places and Times

Daniel Jurafsky and James H. Martin, ["Sequence Labeling", sections 8.1-8.3](https://web.stanford.edu/~jurafsky/slp3/8.pdf)

Matthew Wilkens, “Literary Attention Lag” (2015).

Kim et al., ["What Time Is It? Temporal Analysis of Novels."](https://www.aclweb.org/anthology/2020.emnlp-main.730.pdf)

**Homework 7**

### March 15: Word embeddings

Daniel Jurafsky and James H. Martin, "Vector Semantics & Embeddings": Sections 6.8-6.12

**Homework 8**

### March 22: Image Classification

Daniel Jurafsky and James H. Martin, ["Neural Networks", sections 7.1-7.4](https://web.stanford.edu/~jurafsky/slp3/7.pdf)

Laure Thompson and David Mimno, ["Computational Cut-Ups: The Influence of Dada."](https://mimno.infosci.cornell.edu/papers/JMPS_final.pdf)

Something like this TBA: [Training a CNN classifier using PyTorch.](https://pytorch.org/tutorials/beginner/blitz/cifar10_tutorial.html)

**Homework 9**

### March 29: Transfer Learning and Contextual Embeddings

Read Farhad Manjoo's ["How Do You Know a Human Wrote This?"](https://www.nytimes.com/2020/07/29/opinion/gpt-3-ai-automation.html) Remind me to extract this from the paywall for you.

Spend at least 30 minutes playing [AI Dungeon.](https://play.aidungeon.io/main/landing)

Write a forum post about your experience playing AI Dungeon by going [here](https://transformer.huggingface.co/doc/gpt2-large) and typing the first 50 words. Then hit tab.

Noah A. Smith, ["Contextual Word Representations: Putting Words into Computers"](https://dl.acm.org/doi/pdf/10.1145/3347145)

Optional: Peters et al., ["Deep Contextualized Word Representations."](https://arxiv.org/pdf/1802.05365.pdf)

**Lab** We'll use the HuggingFace implementation of BERT to do simple sentiment classification.

**Homework 10**

### April 5: Starting to Plan Your Project: Experimental Design

When quantitative methods fail in the humanities, how and why do they typically fail?

Nguyen et al., ["How We Do Things With Words: Analyzing Text as Social and Cultural Data."](https://www.frontiersin.org/articles/10.3389/frai.2020.00062/full)

Heather Krause, ["Data Biographies: Getting to Know Your Data."](https://gijn.org/2017/03/27/data-biographies-getting-to-know-your-data/)

Ted Underwood, ["How Not to Do Things with Words."](https://tedunderwood.com/2012/08/25/how-not-to-do-things-with-words/)

**Lab session:** Practice web scraping.

**No homework beyond this point:** you're starting to work on your project.


### April 12: Data "Munging"

Due: Project proposals. You can the forum to describe a specific problem you're facing in your project; we'll use the main course meeting to discuss these.

*Lab session*: Use fuzzy matching to join two datasets.


### April 19: Challenges you're facing; data visualization; representing uncertainty

Use the forum to describe a specific problem you're facing in your project; we'll use the main course meeting to discuss these.

*Lab sessions*: We'll use bootstrap methods to measure uncertainty and probably use GeoPy to create maps.


### April 26: Television studies / challenges you're confronting in your projects
First 30 minutes: Taylor Arnold, Lauren Tilton, Annie Berke, ["Visual Style in Two Network Era Sitcoms"](https://culturalanalytics.org/article/11045-visual-style-in-two-network-era-sitcoms)

The rest of the day, project presentations.


### May 3: Project presentations finish
