# b551-assignment-3-probability-nlp-and-computer-vision-solved
**TO GET THIS SOLUTION VISIT:** [B551 Assignment 3: Probability, NLP and Computer Vision Solved](https://www.ankitcodinghub.com/product/b551-assignment-3-probability-nlp-and-computer-vision-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;100761&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;B551 Assignment 3: Probability, NLP and Computer Vision Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
This assignment will give you a chance to practice probabilistic inference for some real-world problems in natural language processing and computer vision.

<h1>Part 0: Getting started</h1>
You can find your team arrangement by logging into IU Github at https://github.iu.edu/cs-b551fa2022/ and navigating to the repository a3-release. In online-section-groups.md, you should find your name in the corresponding table under Group Assignment Sheet. To get started, clone the github repository using one of the two commands:

git clone git@github.iu.edu:cs-b551-fa2022/a3-release git clone https://github.iu.edu/cs-b551-fa2022/a3-release

<h1>Part 1: Part-of-speech tagging</h1>
A basic problems in Natural Language Processing is <em>part-of-speech</em> <em>tagging</em>, in which the goal is to mark every word in a sentence with its part of speech (noun, verb, adjective, etc.). Sometimes this is easy: a sentence like “Blueberries are blue” clearly consists of a noun, verb, and adjective, since each of these words has only one possible part of speech (e.g., “blueberries” is a noun but can’t be a verb).

But in general, one has to look at all the words in a sentence to figure out the part of speech of any individual word. For example, consider the — grammatically correct! — sentence: “Buffalo buffalo Buffalo buffalo buffalo buffalo Buffalo buffalo.” To figure out what it means, we can parse its parts of speech:

Buffalo&nbsp;&nbsp;&nbsp;&nbsp; buffalo&nbsp;&nbsp;&nbsp;&nbsp; Buffalo&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; buffalo buffalo buffalo&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Buffalo&nbsp;&nbsp;&nbsp;&nbsp; buffalo.

Adjective&nbsp;&nbsp;&nbsp; Noun&nbsp;&nbsp;&nbsp; Adjective&nbsp;&nbsp;&nbsp; Noun&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Verb&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Verb&nbsp;&nbsp;&nbsp;&nbsp; Adjective&nbsp;&nbsp;&nbsp;&nbsp; Noun

(In other words: the buffalo living in Buffalo, NY that are buffaloed (intimidated) by buffalo living in Buffalo,

NY buffalo (intimidate) buffalo living in Buffalo, NY.)

That’s an extreme example, obviously. Here’s a more mundane sentence:

Her&nbsp;&nbsp;&nbsp;&nbsp; position covers&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; a&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; number&nbsp;&nbsp;&nbsp;&nbsp; of&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; daily&nbsp;&nbsp;&nbsp;&nbsp; tasks&nbsp;&nbsp;&nbsp; common&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; to&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; any&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; social director.

DET&nbsp;&nbsp;&nbsp;&nbsp; NOUN&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; VERB DET NOUN ADP ADJ NOUN&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ADJ&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ADP DET&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ADJ&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; NOUN

where DET stands for a determiner, ADP is an adposition, ADJ is an adjective, and ADV is an adverb.<a href="#_ftn1" name="_ftnref1"><sup>[1]</sup></a>Many of these words can be different parts of speech: “position” and “covers” can both be nouns or verbs, for example, and the only way to resolve the ambiguity is to look at the surrounding words. Labeling parts of speech thus involves an understanding of the intended meaning of the words in the sentence, as well as the relationships between the words.

Fortunately, statistical models work amazingly well for NLP problems. Consider the Bayes net shown in Figure 1(a). This Bayes net has random variables <em>S </em>= {<em>S</em><sub>1</sub><em>,…,S<sub>N</sub></em>} and <em>W </em>= {<em>W</em><sub>1</sub><em>,…,W<sub>N</sub></em>}. The <em>W</em>’s represent observed words in a sentence. The <em>S</em>’s represent part of speech tags, so <em>S<sub>i </sub></em>∈ {VERB<em>,</em>NOUN<em>,…</em>}. The arrows between <em>W </em>and <em>S </em>nodes model the relationship between a given observed word and the possible parts of speech it can take on, <em>P</em>(<em>W<sub>i</sub></em>|<em>S<sub>i</sub></em>). (For example, these distributions can model the fact that the word “dog” is a fairly common noun but a very rare verb.) The arrows between <em>S </em>nodes model the probability that a word of one part of speech follows a word of another part of speech, <em>P</em>(<em>S<sub>i</sub></em><sub>+1</sub>|<em>S<sub>i</sub></em>). (For example, these arrows can model the fact that verbs are very likely to follow nouns, but are unlikely to follow adjectives.)

<em>Data. </em>To help you with this assignment, we’ve prepared a large corpus of labeled training and testing data. Each line consists of a sentence, and each word is followed by one of 12 part-of-speech tags: ADJ (adjective), ADV (adverb), ADP (adposition), CONJ (conjunction), DET (determiner), NOUN, NUM (number), PRON (pronoun), PRT (particle), VERB, X (foreign word), and . (punctuation mark).<a href="#_ftn2" name="_ftnref2"><sup>[2]</sup></a>

2

(a)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; (b)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; (c)

Figure 1: Bayes Nets for part of speech tagging: (a) HMM, and (b) simplified model, and (c) complicated model.

<em>What to do. </em>Your goal in this part is to implement part-of-speech tagging in Python, using Bayes networks.

<ol>
<li>To get started, consider the simplified Bayes net in Figure 1(b). To perform part-of-speech tagging,we’ll want to estimate the most-probable tag <em>s</em><sup>∗</sup><em><sub>i </sub></em>for each word <em>W<sub>i</sub></em>,</li>
</ol>
<em>s</em><sup>∗</sup><em><sub>i </sub></em>= argmax<em>P</em>(<em>S<sub>i </sub></em>= <em>s<sub>i</sub></em>|<em>W</em>)<em>.</em>

<em>s<sub>i</sub></em>

Implement part-of-speech tagging using this simple model.

<ol start="2">
<li>Now consider Figure 1(a), a richer Bayes net that incorporates dependencies between words. ImplementViterbi to find the maximum a posteriori (MAP) labeling for the sentence,</li>
</ol>
) = arg max&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <em>.</em>

<ol start="3">
<li>Consider the Bayes Net of Figure 1c, which could be a better model because it incorporates richerdependencies between words. But it’s not an HMM, so we can’t use Viterbi. Implement Gibbs Sampling to sample from the posterior distribution of Fig 1c, <em>P</em>(<em>S</em>|<em>W</em>). Then estimate the best labeling for each word (by picking the maximum marginal for each word, <em>s</em><sup>∗</sup><em><sub>i </sub></em>= argmax<em><sub>s</sub></em><em><sub>i </sub>P</em>(<em>S<sub>i </sub></em>= <em>s<sub>i</sub></em>|<em>W</em>)<em>. </em>(To do this, just generate many (thousands?) of samples and, for each individual word, check which part of speech occurred most often.)</li>
</ol>
Your program should take as input a training filename and a testing filename. The program should use the training corpus to estimate parameters, and then display the output of Steps 1-3 on each sentence in the testing file. For the result generated by each of the three approaches (Simple, HMM, Complex), as well as for the ground truth result, your program should output the logarithm of the joint probability <em>P</em>(<em>S,W</em>) for each solution it finds under each of the three models in Figure 1. It should also display a running evaluation showing the percentage of words and whole sentences that have been labeled correctly so far. For example:

[djcran@raichu djc-sol]$ python3 ./label.py training_file testing_file Learning model…

Loading test data…

Testing classifiers…

<table width="577">
<tbody>
<tr>
<td width="126">&nbsp;</td>
<td width="213">Simple&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; HMM Complex Magnus</td>
<td width="238">ab integro seclorum nascitur ordo .</td>
</tr>
<tr>
<td width="126">0. Ground truth</td>
<td width="213">-48.52 -64.33&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; -73.43&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; noun</td>
<td width="238">verb&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; adv&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; conj&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; noun noun .</td>
</tr>
<tr>
<td width="126">1. Simplified</td>
<td width="213">-47.29 -66.74&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; -75.29&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; noun</td>
<td width="238">noun&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; noun&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; adv&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; verb noun .</td>
</tr>
<tr>
<td width="126">2. HMM</td>
<td width="213">-47.48 -63.83&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; -74.12&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; noun</td>
<td width="238">verb&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; adj&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; conj&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; noun verb .</td>
</tr>
<tr>
<td width="126">&nbsp;&nbsp;&nbsp;&nbsp; 3.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Complex</td>
<td width="213">-47.50 -64.21&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; -72.02&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; noun</td>
<td width="238">verb&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; adv&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; conj&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; noun noun .</td>
</tr>
</tbody>
</table>
==&gt; So far scored 1 sentences with 17 words.

100 tags, depending on the language of interest – that carry finer-grained information like the tense and mood of verbs, whether nouns are singular or plural, etc. In this assignment we’ve simplified the set of tags to the 12 described here; the simple tag set is due to Petrov, Das and McDonald, and is discussed in detail in their 2012 LREC paper if you’re interested.

3

Words correct:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sentences correct:

<ol>
<li>Ground truth 00%&nbsp;&nbsp; 100.00%</li>
<li>Simplified 85%&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 0.00%</li>
<li>HMM 43%&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 0.00%</li>
<li>Complex 00%&nbsp;&nbsp; 100.00%</li>
</ol>
We’ve already implemented some skeleton code to get you started, in three files: label.py, which is the main program, pos scorer.py, which has the scoring code, and pos solver.py, which will contain the actual part-ofspeech estimation code. You should only modify the latter of these files; the current version of pos solver.py we’ve supplied is very simple, as you’ll see. In your report, please make sure to include your results (accuracies) for each technique on the test file we’ve supplied, bc.test. Your code should finish within about 10 minutes.

<h1>Part 2: Reading text</h1>
To show the versatility of HMMs, let’s try applying them to another problem; if you’re careful and you plan ahead, you can probably re-use much of your code from Part 1 to solve this problem. Our goal is to recognize text in an image – e.g., to recognize that Figure 2 says “It is so ordered.” But the images are noisy, so any particular letter may be difficult to recognize. However, if we make the assumption that these images have English words and sentences, we can use statistical properties of the language to resolve ambiguities.

Figure 3: Our goal is to extract text from a noisy scanned image of a document.

We’ll assume that all the text in our images has the same fixed-width font of the same size. In particular, each letter fits in a box that’s 16 pixels wide and 25 pixels tall. We’ll also assume that our documents only have the 26 uppercase latin characters, the 26 lowercase characters, the 10 digits, spaces, and 7 punctuation symbols, (),.-!?’”. Suppose we’re trying to recognize a text string with <em>n</em> characters, so we have <em>n</em> observed variables (the subimage corresponding to each letter) <em>O</em><sub>1</sub><em>,</em> <em>…,</em> <em>O<sub>n</sub></em> and <em>n</em> hidden variables, <em>l</em><sub>1</sub><em>…,</em> <em>l<sub>n</sub></em>, which are the letters we want to recognize. We’re thus interested in <em>P</em> (<em>l</em><sub>1</sub><em>,</em> <em>…,</em> <em>l<sub>n</sub></em>|<em>O</em><sub>1</sub><em>,</em> <em>…,</em> <em>O<sub>n</sub></em>). As in part 1, we can rewrite this using Bayes’ Law, estimate <em>P</em> (<em>O<sub>i</sub></em>|<em>l<sub>i</sub></em>) and <em>P</em> (<em>l<sub>i</sub></em>|<em>l<sub>i</sub></em><sub>−1</sub>) from training data, then use probabilistic inference to estimate the posterior, in order to recognize letters.

<em>What</em> <em>to</em> <em>do.</em> Write a program called image2text.py that is called like this:

python3 ./image2text.py train-image-file.png train-text.txt test-image-file.png

The program should load in the train-image-file, which contains images of letters to use for training (we’ve supplied one for you). It should also load in the text training file, which is simply some text document that is representative of the language (English, in this case) that will be recognized. (The training file from Part 1 could be a good choice). Then, it should use the classifier it has learned to detect the text in test-image-file.png, using (1) the simple Bayes net of Figure 1b and (2) the HMM of Fig 1a with MAP inference (Viterbi). The last two lines of output from your program should be these two results, as follows:

[djcran@tank]$ python3 ./image2text.py train-image-file.png train-text.txt test-image-file.png

Simple: 1t 1s so orcerec. HMM: It is so ordered.

4

<em>Hints.</em> We’ve supplied you with skeleton code that takes care of all the image I/O for you, so you don’t have to worry about any image processing routines. The skeleton code converts the images into simple Python list-of-lists data structures that represents the characters as a 2-d grid of black and white dots. You’ll need to define an HMM and estimate its parameters from training data. The transition and initial state probabilities should be easy to estimate from the text training data. For the emission probability, we suggest using a simple naive Bayes classifier. The courier-train.png file contains a perfect (noise-free) version of each letter. The text strings your program will encounter will have nearly these same letters, but they may be corrupted with noise. If we assume that <em>m</em>% of the pixels are noisy, then a naive Bayes classifier could assume that each pixel of a given noisy image of a letter will match the corresponding pixel in the reference letter with probability (100 − <em>m</em>)%.

<h2>What to turn in</h2>
Create a private repository using the name you found in the Group Assignment Sheet, and keep the same directory structure as in a3-release (i.e., separating the programs into Part1 and Part2). Make sure that you stick to this naming scheme and directory structure so that our autograder can locate your submission correctly. And make sure it is private (not internal or public) so others will not see your submission. Turn in the required programs on GitHub (remember to add, commit, push) — we’ll grade whatever version you’ve put there as of 11:59:59PM on the due date. To make sure that the latest version of your work has been accepted by GitHub, you can log into the github.iu.edu website and browse the code online.

5

<a href="#_ftnref1" name="_ftn1">[1]</a> If you didn’t know the term “adposition”, neither did I. The adpositions in English are prepositions; in many languages, there are postpositions too. But you won’t need to understand the linguistic theory between these parts of speech to complete the assignment; if you’re curious, check out the “Part of Speech” Wikipedia article for some background.

<a href="#_ftnref2" name="_ftn2">[2]</a> This dataset is based on the Brown corpus. Modern part-of-speech taggers often use a much larger set of tags – often over
