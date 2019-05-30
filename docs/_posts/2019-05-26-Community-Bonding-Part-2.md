---
layout: post
title: Community Bonding Period - Part-2
comments: false
categories: [GSoC]
---

With the community bonding period done, the actual coding phase has started. As mentioned in my previous blog post, in this post I will be talking about the modifications I have made, what I worked on in the second half of my community bonding period and what I will be doing for the next week.

In the `pyspotlight` module, the main modification I did and perhaps the only change I made was to make annotations possible by using the online API, instead of requiring a local version of the API. In the `conllu` module the formatting for parsing was changed in accordance to the .conll files being output by SyntaxNet. Also a special parse function for files which represented a single sentence was created.

### Hearst Patterns

In the later half of the community bonding period, I spent time understanding hearst patterns. Hearst patterns can help us identify relations between words ie, r(a, b, n) where 'a' and 'b' are the two words. ex, 'Person ABC' , 'New York', 'birthPlace'. These can be found either statistically, like most modern NLP techniques or using specific patterns to search. Intuitively a pattern wise search would be less performing, because they are highly constrained, however studies have shown otherwise \[1](https://aclweb.org/anthology/P18-2057). The methods do take advantage of the POS tags of the words.

My tasks for the first week are as follows:

In the first week, I would concentrating on using hearst patterns to be able to identify relations. As of now I would be concentrating on a few number of relations. The idea would be to understand how well it does over a large dataset and whether in order to find a relation, it would not require to develop a large number of specific patterns. Another approach would be the statistic approach and see if a model can be created to do the following and whether this can be easily modified and replicated for all other types of relations.

Another important part would be understanding how having a dependent parse of the sentence can change the output of the results VS a simple surface POS (which can both be offerred by SyntaxNet)

In the next blog post (coming up after the first week), I will be talking about the program which would be developed for this and all the prelimnaries for the experiment. The codebase for the following can be found at `github.com/sahitpj/GSoC-codebase`

Cheers!