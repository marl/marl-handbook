# Writing

Technical writing is not easy, and very few of us ever receive direct training.
While a course on technical writing can be worthwhile, there is much to the subject, and we will not cover everything you need to know in this
section.

The number one reason for a paper to be rejected is that the reviewers don't understand it.
This section will outline just the basics and provide a few easy tips for improving your writing with an emphasis on clarity.


## Paper structure

There is no single recipe for a good paper structure, but most will have an organization something like the following:

0. Abstract
1. Introduction
2. Background / related work / etc
3. Methods
4. Results
5. Discussion / conclusion

The naming and ordering of these sections may vary by discipline or publication venue---e.g., some communities tend to put *related work* sections at
the end instead of the beginning---but the breakdown by content is roughly consistent.

Let's go through each of these sections in turn.

### Abstract

A good abstract should tell the reader two things: 1) what the contribution of your work is, and 2) why a reader should care about it.
Very often, this is as much of a paper as a person will ever read, so it is important to make it clear and concise.
Most publication venues will have constraints on the length of an abstract (e.g., 200 words) but no specific guidelines beyond that.

In general, focus on the take-away message of your work, rather than reporting specific details.
For example, the following abstract provides too much detail and does not clearly convey the take-away message:

```{admonition} An abstract that needs improvement
:class: danger

Some garbage abstract TBD
```

It could be improved as follows:

```{admonition} An improved abstract
:class: tip

A better example of an abstract would be something like this
```

### Introduction

The introduction section is not just a rehash of the abstract.
It should give a bit more background on the problem or subject you are addressing, and articulate your approach and contribution at a high level.

Some authors like to include a dedicated subsection (or at least a paragraph) at the end to enumerate specific contributions.

If your paper is on the more mathematical or theoretical side, it may also be appropriate to include a subsection that quickly introduces common
notation and terminology.
This is not very common for the kind of work we typically do in MARL, but every so often it is appropriate.

```{note} 
Unless your paper is long (i.e., more than 10 pages), you should not have a "roadmap" paragraph describing what is in each section.
Oftentimes this is not a good use of space, and a reader can figure out by skimming the paper anyway.
```


### Background and related work

This section is primarily used to help the reader understand where your contribution sits relative to the prior literature on the topic.
A good background section should not only describe the prior work, but give clear and concise explanations of how your work relates to the prior literature.
Often this means identifying the gaps in the prior work that your work is filling, or the limitations of the prior work that your work is addressing.
It can also mean identifying differences in context between your work and prior work.
All of these things are helpful to the reader in understanding what exactly your contribution is.



### Methods

This is usually considered the *core* of the paper: it's where you describe what you did and how you did it.
This is probably the section you're most excited about writing.

You might find it helpful to include specific subsections here for experiment or evaluation design, data sets used, and other implementation
details.
Sometimes this flows better when integrated into the following section (*Results*, which could also be titled *Experiments*), so use your best judgment.

When describing experiments, it is critical to clearly articulate to the reader **what question is the experiment designed to answer?**
Sometimes this is obvious, but often it is not.
Being explicit on this point never hurts, and it will make the results section easier to write.

### Results

This is where you report the outcomes of your work.
This could mean reporting tables of accuracy measurements, outcomes of survey data, or any number of other things.

Keep this section concise and factual.  It is not the place to provide interpretation of your results---that comes next---but just to state what
they are.

Often you will be conducting multiple experiments or evaluations, or asking several questions articulated in the previous section.
You might find it useful to break the results section down into subsections corresponding to each research question or experiment.

### Discussion and conclusion

A discussion section should not be a rehash of the introduction or results section.
Rather, it should be a place to provide interpretation of the results, provide context, and discuss their implications.

It is also a good place to discuss limitations of your work and outline future directions.

### Other parts

- Tag your paper and repository at each submission!

## Advice for clear writing


**Assume that your readers are not paying attention.**

Your first readers, outside your co-authors and immediate colleagues, will be the reviewers.
If you are submitting your work to a conference, you can expect that each reviewer is reading your paper along with 3-5 other papers in their batch,
and will have limited time and attention span.
**It is your responsibility to make it easy for them to understand your work.**
Sometimes this means stating obvious facts, but always err on the side of clarity rather than hoping that the reader will "just figure it out" on
their own.


**Keep sentences and paragraphs short.**

The longer a sentence is, the more likely it is to be confusing.
Even if it is not confusing, readers can become distracted or lose track of the point you are trying to make.
Avoid parenthetical and complicated sentence structures.

The same goes for paragraphs and sections: try to keep things as brief as possible without sacrificing important content.


````{admonition} Concise writing is hard work
:class: tip

```{epigraph}

*Je n'ai fait celle-ci plus longue que parce que je n'ai pas eu le loisir de la faire plus courte.*

Translation:

*I have made this longer than usual because I have not had time to make it shorter.*

-- Blaise Pascal, 1657
```
````

**Put the important stuff first!**

Expect that most readers will be skimming your paper, at least on a first read.
They may jump from one section to another to try to get a sense of whether your work is relevant to them.
Usually this means that they will read the beginning of a section or paragraph, but maybe not the middle and end.

To maximize your chances of the reader understanding your work: organize your sentences and paragraphs so that the most important parts come first.
```{admonition} A sentence that could be improved
:class: danger

Some garbage sentence TBD
```

Could be improved

```{admonition} An improved version of the same sentence
:class: tip

TBD
```


**Don't expect readers to see things that aren't there: be explicit.**

**Citations are punctuation, not a part of speech.**






## Checklist for reviewing your work
    - [ ] Free of typos.  Use a spell checker!
    - [ ] All mathematical notation is defined prior to its first use
    - [ ] All acronyms and abbreviations are defined prior to use
    - [ ] All figures and tables are referenced in the text
    - [ ] All figures have readable font sizes (at least footnote size relative to main text)
    - [ ] All figures have descriptive captions

## LaTeX-specific tips
    - In math mode, use `\ell` instead of `l` for the letter "l"
    - Use `\left` and `\right` for all parentheses, brackets, and braces.  This will make them scale to 
      the size of the content inside them.
    - Use `\ref` (or `\cref` with the `cleveref` package, or `\eqref`) for all references to figures, tables, and equations.  This ensures that all numbering stays consistent as things change.
    - Use `booktabs` and do not include extraneous lines in tables (`tabular` environments).  Use `\toprule`, `\midrule`, and `\bottomrule` to separate the header from the body, and the body from the footer.

