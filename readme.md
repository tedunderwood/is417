IS417 Data Science in the Humanities
====================================

Human culture provides an ideal testbed for students exploring data science, because the interpretive challenges that lurk beneath the surface in other domains become starkly visible here. For instance, cultural materials start out as unstructured texts, images, or sound files, forcing explicit decisions about data modeling and feature extraction. Humanistic questions also highlight the importance of interpreting statistical models in relation to a social context. Last but not least: songs, poems, and stories confront us with vivid problems that are inherently fun to explore.

A semester of previous exposure to some programming language is a prerequisite for this course; the programming language you've used doesn't need to be Python, but you should be comfortable with concepts like "variable assignment" and "loops."

How to use this course
----------------------

Most aspects of the course will run through [the Moodle page](learn.illinois.edu); that's where you can connect to Zoom, upload assignments, and write forum posts.

But I'll also be distributing Jupyter notebooks and supporting data files. In most cases, it will be easiest to distribute those through GitHub.

So you might start by [installing git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git). Then open [a command line,]((https://melaniewalsh.github.io/Intro-Cultural-Analytics/features/Command-Line/The-Command-Line.html)) ```cd```` to a directory where you want to place ```is417/``` as a subfolder, and clone the repository by saying:

    git clone https://github.com/tedunderwood/is417.git

Later, when new materials have been added to this folder, you can get the materials by navigating to the ```is417``` folder and saying:

    git pull origin main

The files will automatically be placed in appropriate folders, which makes this a lot easier than downloading things from Moodle.

You might also consider creating a subfolder within is417 named with your netID (e.g. for me it would be ```tunder/```), and keeping your homework assignments (just the ```.ipynb``` files) in that folder. At a later stage of the semester, this might make it easier to share your homework with me so I can help you debug.

January 25: Introduction to Jupyter and Python
----------------------------------------------

**What are the humanities?**
Familiar answers, from 4Humanities:
https://4humanities.org/2014/12/what-are-the-humanities/

Puzzling evidence from the Google ngram viewer:
https://rb.gy/1rbtj2

**What happens when the humanities meet data science?**
Mohr, Wagner-Pacifici, and Breiger, ["Toward a Computational Hermeneutics."](https://journals.sagepub.com/doi/full/10.1177/2053951715613809)

We'll discuss this article in some depth.

Campo-Rembado and Oakley, ["How 20th Century Fox Uses ML to Predict a Movie Audience."](https://cloud.google.com/blog/products/ai-machine-learning/how-20th-century-fox-uses-ml-to-predict-a-movie-audience)

Don't worry deeply about the technical details here; I'm not planning to discuss this piece in depth--just giving you a glimpse of what's possible.

**Lab session**

Walsh, ["The Command Line"](https://melaniewalsh.github.io/Intro-Cultural-Analytics/features/Command-Line/The-Command-Line.html) and ["How To Use Jupyer Notebooks"](https://melaniewalsh.github.io/Intro-Cultural-Analytics/features/Python/How-to-Use-Jupyter-Notebooks.html)

Install git and clone the IS417 repository. This will give you
```Milne_ALostMasterpiece.txt``` in the ```texts/``` directory, and
```simple_word_counting.ipynb``` in the ```code/``` subdirectory.

See if you can run ```simple_word_counting.ipynb.```

**Homework 1:** Write code blocks that
a) check whether a word contains any repeated letters,
b) test whether two words are anagrams,
c) (optional, extra) find all common English words that are anagrams for a given string.

If you don't have previous experience with Python, you may want to work through [sections 2-7 of "The Python Tutorial"](https://docs.python.org/3/tutorial/) before attempting the homework. Other introductory books and online tutorials could work equally well; Melanie Walsh has good chapters on Lists, Loops, String Methods, and Dictionaries that can be downloaded as notebooks.

February 1: Descriptive and Inferential Statistics with Pandas
--------------------------------------------------------------

read Anelise Hanson Shrout, "(Re)Humanizing Data: Digitally Navigating the Bellevue Almshouse."
read Melanie Walsh, "Pandas Basics."

Before class, work through the notebook ```MoviesAndStatistics.ipynb.```

David Robinson, ["Text Analysis of Trump's Tweets Confirms He Writes Only the (Angrier) Android Half."](http://varianceexplained.org/r/trump-tweets/)

Benjamin Schmidt, ["Comparing Corpuses by Word Use."](http://sappingattention.blogspot.com/2011/10/comparing-corpuses-by-word-use.html)

optional background: Ted Dunning, ["Accurate Methods for the Statistics of Surprise and Coincidence."](https://www.aclweb.org/anthology/J93-1003.pdf)

**Lab session:**

Can we improve on Robinson's analysis, and find words that are significantly over-represented in the Android tweets?

**Homework 2:**

Questions about movie dialogue, by period, genre, and character gender.

If you need more background on descriptive and inferential statistics, I recommend the free [*OpenIntro Statistics.*](https://leanpub.com/openintro-statistics)


February 8: Probability and statistical learning
------------------------------------------------


February 15: High-Dimensional Space: Where the Humanities Happen
---------------------------------------------------------------

Daniel Jurafsky and James H. Martin, "Vector Semantics & Embeddings": Sections 6-6.4

Victor Powell, [“Principal component analysis explained visually.”](https://setosa.io/ev/principal-component-analysis/)

Alison et al., “Quantitative Formalism.”

Before class, work through the notebook ```MovieSimilarity.ipynb```

Optional: Matt Daniels, ["The Language of Hip Hop."](https://pudding.cool/2017/09/hip-hop-words/)

**Lab session**:

We'll perform principal component analysis on movies, and measure the similarity of words in "dialogue space."

**Homework 3:**

Principal component analysis on movie genres.

February 22: How to Learn in High-Dimensional Space: Logistic Regression
------------------------------------------------------------------------

For intuition, Stephanie Yee and Tony Chu, [“A Visual Introduction to Machine Learning.”](http://www.r2d3.us/visual-intro-to-machine-learning-part-1/) You may also enjoy ["Part 2: Model Tuning and the Bias-Variance Tradeoff."](http://www.r2d3.us/visual-intro-to-machine-learning-part-2/)

James, Witten, Hastie, and Tibshirani, "2. Statistical Learning," "4. Classification," and "5.1 Cross-Validation" from *An Introduction to Statistical Learning.*

As you read these chapters, work through the paired notebook ```HumanitiesML.ipynb," which will show you how to apply the principles explained in James et al. using Python rather than the R they use.

Vincent Spruyt, ["The Curse of Dimensionality in Classification."](https://www.visiondummy.com/2014/04/curse-dimensionality-affect-classification/)

**Lab session**

We'll measure the strength of gender stereotypes in movie dialogue.

**Homework 4:**

Do gender stereotypes change across time?


March 1: Topic Modeling
---------------------------

March 8: Beyond Bags of Words: People, Places and Times
-----------------------------------------------------------

Daniel Jurafsky and James H. Martin, ["Sequence Labeling", sections 8.1-8.3](https://web.stanford.edu/~jurafsky/slp3/8.pdf)

Matthew Wilkens, “Literary Attention Lag” (2015).

Kim et al., ["What Time Is It? Temporal Analysis of Novels."](https://www.aclweb.org/anthology/2020.emnlp-main.730.pdf)


March 15: Word embeddings
--------------------------

Daniel Jurafsky and James H. Martin, "Vector Semantics & Embeddings": Sections 6.8-6.12


March 22: Image Classification
------------------------------

Daniel Jurafsky and James H. Martin, ["Neural Networks", sections 7.1-7.4](https://web.stanford.edu/~jurafsky/slp3/7.pdf)

Laure Thompson and David Mimno, ["Computational Cut-Ups: The Influence of Dada."](https://mimno.infosci.cornell.edu/papers/JMPS_final.pdf)

Something like this TBA: [Training a CNN classifier using PyTorch.](https://pytorch.org/tutorials/beginner/blitz/cifar10_tutorial.html)


March 29: Transfer Learning and Contextual Embeddings
-----------------------------------------------------

Noah A. Smith, ["Contextual Word Representations: Putting Words into Computers"](https://dl.acm.org/doi/pdf/10.1145/3347145)
Optional: Peters et al., ["Deep Contextualized Word Representations."](https://arxiv.org/pdf/1802.05365.pdf)

We'll use the HuggingFace implementation of BERT to do simple sentiment classification.


April 5: Starting to Plan Your Project: Experimental Design
------------------------------------------------------------

When quantitative methods fail in the humanities, how and why do they typically fail?

Nguyen et al., ["How We Do Things With Words: Analyzing Text as Social and Cultural Data."](https://www.frontiersin.org/articles/10.3389/frai.2020.00062/full)

Heather Krause, ["Data Biographies: Getting to Know Your Data."](https://gijn.org/2017/03/27/data-biographies-getting-to-know-your-data/)

Ted Underwood, ["How Not to Do Things with Words."](https://tedunderwood.com/2012/08/25/how-not-to-do-things-with-words/)

*Lab session*: Practice web scraping.

No homework: you're starting to work on your project.


April 12: Data "Munging"
--------------------------

Due: Project proposals. You can the forum to describe a specific problem you're facing in your project; we'll use the main course meeting to discuss these.

*Lab session*: Use fuzzy matching to join two datasets.


April 19: Challenges you're facing; data visualization; representing uncertainty
-------------------------------------------------------------------------------

Use the forum to describe a specific problem you're facing in your project; we'll use the main course meeting to discuss these.

*Lab sessions*: We'll use bootstrap methods to measure uncertainty and probably use GeoPy to create maps.


April 26: Television studies / challenges you're confronting in your projects
------------------------------------------------------------------------------
First 30 minutes: Taylor Arnold, Lauren Tilton, Annie Berke, ["Visual Style in Two Network Era Sitcoms"](https://culturalanalytics.org/article/11045-visual-style-in-two-network-era-sitcoms)

The rest of the day, project presentations.


May 3: Project presentations finish
-------------------------------------




