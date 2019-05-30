---
layout: post
title: Introduction & Community Bonding Period - Part-1
comments: false
categories: [GSoC]
---

The following blog is an account of the GSoC project taken by me under DBpedia. I would like to thank Mariano Rico for mentoring and who will be following me through this journey. A few details about this project :- The main idea of this project is use syntactic methods (syntax parsers) coupled with other linguistic based algorithms in order to help generate triples from information abstracts. DBpedia has created a large web graph using the following data which can be found on their website. We wish to provide a sort of automation to finding triples which can be added to this webgraph. The other details can be found in my proposal.

The firt phase of GSoC is the Community bonding period which extends till late May. In this phase, prelimnaries to that project are taken care of. Given I have reached the halfway point of this phase, I thought of talking about what all I have done and what I will work on in the near future. 

### Task-1 : Spotlight

The first prelimnary tasks include understanding DBpedia Spotlight. Spotlight is an annotating tool, which when given an abstract or a sentence can annotate words, given their presence in the DBpedia web graph or an instance of it is present. Understanding this would be important, given that this tool will be necessary for generating triples and mapping these words to the already existant forms present in the DBpedia web graph. 

Given this project will be mostly be done in Python, it was necessary to have a python wrapper for the following. Luckily `pyspotlight` exists, to which I made a few modifications to it to suit the project needs.

<b>link</b> - https://github.com/sahitpj/pyspotlight

<br>

### Task-2 : Exploring methods for the project

On the other hand it was also necessary to come with a good idea of how we are to proceed with the overall project. To be more specific, exploring algorithms to use syntactic methods for triple extraction was necessary. I managed to get hold of a few good papers given to me by my mentor, and thus have gone through them.

### Task-3 : Conll parsing

Another important thing which was to be taken care at the earliest would be identifying tree query languages, given that the syntactic parsers generally give the parse output in the form of a `.conll` file. Given most of these libraies are present in other languages such as Java and that python libraries don't offer much flexibility, it was important to find a suitable library for the project. After going through Universal Dependencies and Github for such packages, I finally managed to find a python library for the following. This library is now being modified to suit the needs of the project. The link to the this library and the original library can be found at the link below.

<b>link</b> - https://github.com/sahitpj/conll

<br>

The Code-base of this project will be hosted on Github shortly. Details of pyspotlight and conll modifications will be put in the next blog post (decided to keep this short and sweet). Do check out my other blog posts!

Cheers!