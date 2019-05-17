---
layout: post
title: Introduction & Community Bonding Period - Part-1
comments: false
categories: [GSoC]
---

The following blog is an account of my GSoC project under DBpedia. I would like to thank Mariano Rico for mentoring and who will be following me through this journey. A little detail about my project :- The main idea of this project is use syntactic methods (syntax parsers) coupled with other linguistic based algorithms in order to help generate triples from information abstracts. DBpedia has created a large web graph using the following data which can be found fromn their website. We wish to provide a sort of automation to finding triples which can be added to this webgraph. The other details can be found in my proposal.


The Community bonding period extends till late May, and given this is a sort of half way point to it, I thought of accounting what all I have done and what I will work on in the near future. 

### Task-1 : Spotlight

The first prelimnary tasks include Understanding DBpedia Spotlight. Spotlight is an annotating tool, which given an abstract or a sentences can annotate words given their presence in the DBpedia web graph or an instance of it is present. Understanding this would be important, given that this tool will be necessary for generating triples. 

Given this project will be mostly be done in Python, it was necessary to have a python wrapper for the following. Luckily `pyspotlight` exists, to which I made a few modifications to the projects needs.

<b>link</b> - https://github.com/sahitpj/pyspotlight

<br>

### Task-2 : Exploring methods for the project

Side by side, exploring methods to actually finding methods was nececssary. A good finding which my mentor had told me about were Hearst patterns, which talks about linguistic patterns which can be found in text statistically. The link to the paper can be found [here](https://research.fb.com/publications/hearst-patterns-revisited-automatic-hypernym-detection-from-large-text-corpora/)

### Task-3 : Conll parsing

Another thing which was to be taken care for now would be identifying tree query languages given that the syntactic parsers generallly give the parse output in the form of a `.conll` file. Given most of these librraies are present in other languages such as Java and python libraries don't offer much flexibility, the following reposiory is being modified to suit the nature of the project.


<b>link</b> - https://github.com/sahitpj/conll

<br>

Overall the progress of the project seems to be on track. The Code-base of this project will be hosted on Github shortly. Details of pyspotlight and conll modifications will be put in the next blog post (decided to keep this short and sweet). Do check out my other blog posts!

Cheers!