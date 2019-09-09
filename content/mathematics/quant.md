---
title: "Diagonalization, Quantification, and Definability"
date: 2019-09-08T20:12:23-07:00
draft: false
---

I've been thinking about different ways to talk about quantification. 

Specifically, I've been thinking about two different semantic interpretations of the quantifiers. On the *objectual* interpretation of the quantifiers, \\( \forall x \phi(x) \\) is true if for every object \\(d\\) in the domain, \\(\phi[d/x]\\) is true. This is usually spelled out in terms of variable assignments to distinguish it more sharply from the other interpretation. On the *substitutional* interpretation of the quantifiers \\( \Pi x \phi(x) \\) is true if for every closed term \\(t\\) of the language, \\(\phi[t/x]\\) is true. 

Substitutional quantification is language-relative. The truth of a given quantified sentence depends on what closed terms are available in the language. One might think this runs into particular problems when we want to talk about the truth of quantified sentences in uncountable structures, like say, the reals. 

For any reasonable (countable) language of the reals, say \\(L\\) the language of ordered rings \\( \\{0, 1, -, +, \cdot, <\\}\\), there are real numbers in \\(\mathbb{R}\\) which are not definable over \\(L\\). It's easy to see that substitutional quantification and objectual quantification must come apart in such a structure, even if we expand substitutional quantification to allow quantification over all definable elements. 

[Hugly and Sayward](https://www.jstor.org/stable/20117947) think arguments which aim to show that some elements of the reals must be unspecifiable proceed a little too quickly: 

> It is sometimes assumed that since the expressions in a language are only denumerably many, in contrast to the indenumerability of the reals, some reals - indeed indenumerably many of them - are unspecifiable. But the relevant proof establishes only that no function maps the reals into the expressions of a language, from which nothing about specifiability follows. It is worth noting that the diagonal argument constituting the proof itself shows how to construct a specification of yet another real. (See Lorenzen (1971, pp. 35-37) for a suggestive discussion of this point.)

> To give an example of this in a minimally complex way, consider the anatagous point for integer sets. Let L be a list of all integer set specifications currently available to us. Then there is this further specification, 'the integer set including integer n just in case n is not a member of the integer set denoted by the nth listed integer set specification'. With this turn of phrase we extend our language to contain a specification of an integer set for which we antecedently possessed no specification (since the assertion that we antecedently possessed this specification leads to a contradiction as in standard diagonalization proofs).

> So, although we may not possess the means of showing that there are no utterly unspecifiable reals, we also do not have this conception forced upon us by the proofs which serve to show that no language (=possible vehicle of communication) can exhaus- tively specify the reals.

I think their reply goes seriously wrong. In what sense does a diagonalization argument give a specification of yet another real? [Timothy Gowers](https://twitter.com/wtgowers/status/1168983651415142400) recently repeated this claim, which inspired this post. 

First, note that in an obvious sense, for any real \\(r \in \mathbb{R}\\), there is an expansion of the language \\(L\\) in which \\(r\\) is specifiable: just add a constant and let its interpretation be \\(r\\)! But this is not the kind of specification Hugly and Sayward seem to have in mind. They seem to mean, a specification in some ``natural`` expansion of the language. A typical expansion by constant doesn't work. This claim, to me, seems to rely on a certain intuition about naming. One might think that, if there are two identical blue books on my coffee table and I proclaim: 'Let Fred be the name of a blue book on the table,' I haven't really named anything at all, despite my proclaiming otherwise. 
