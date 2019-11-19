# ![](IMG_3320) 

## Fatimah Aloqayli


## Introduction

In this work manipulate and analyze the language data. The concept behind grouping the articles,
legal documents, news etc, , based on their relevance.

As an example:
if Iam a part of a big legal firm (e.g. Jones Day, Gibson Dunn), where I
need to find out the relevant documents from thousands of pages!

These and many other similar tasks are not trivial for human. This
is where **Natural Language Processing (NLP)** can help, when we
are dealing with text data!

By definition, **Natural-language processing (NLP)** is an area of
computer science and artificial intelligence, concerned with the
interactions between computers and human (natural) languages, in
particular how to program computers to fruitfully process large amounts
of natural language data.

## problem statment 

we want to do the following:
1. compile the documents is some fashion
2. get feature from the documents
3. compare their features for similarity


where we have the following query strings:
1. "tennis match"
2. "88 thousand people!"
3. "the plastic container; see <img src='drawing.jpg' alt=''>"

And 20 documents 

## The solution steps

A simple way to featurize the text document is to do the word count. We
can transform “text” into a vectorized word counts. In order to do this,
we basically create a vector count of all the possible words in all the
documents. We then count how many times those words appear in each
document. 

A document represented as a vector of word counts is called “Bag of
Words”. Treating each document as a vector of features is useful
because, once, we have the bag of words vectors, we can perform
mathematical operations on them. For example, we can compute
cosine similarity using the equation below. We can also compute other
similarity metrics in order to figure out how similar two text documents
are to each other.

We improve the Bag of Words (BoW) by adjusting word counts, based on their frequency in corpus (a collection of written text or a group of all the documents). and we use TF-IDF (Term Frequency - Inverse Document Frequency) in order to do this.

Term Frequency (TF) measures how frequently a term occurs in a document. TF(t, d) depends upon the number of occurrences of term “t” in the document “d”. This suggest how important the term is within that document.
Inverse Document Frequency (IDF) measures the importance of the term in the corpus (group of all the documents).

