---
title: "Quantification and Definability"
date: 2019-09-08T20:12:23-07:00
draft: false
---

I've been thinking about different ways to talk about quantification. 

Specifically, I've been thinking about two different semantic interpretations of the quantifiers. On the *objectual* interpretation of the quantifiers, \\( \forall x \phi(x) \\) is true if for every object \\(d\\) in the domain, \\(\phi[d/x]\\) is true. This is usually spelled out in terms of variable assignments to distinguish it more sharply from the other interpretation. On the *substitutional* interpretation of the quantifiers \\( \forall x \phi(x) \\) is true if for every closed term \\(t\\) of the language, \\(\phi[t/x]\\) is true. 

Substitutional quantification is language-relative. The truth of a given quantified sentence depends on what closed terms are available in the language. One might think this runs into particular problems when we want to talk about the truth of quantified sentences in uncountable structures, like say, the reals. 

For any reasonable (countable) language of the reals, say \\(L\\) the language of ordered rings \\( \\{0, 1, -, +, \cdot, <\\}\\), there are real numbers in \\(\mathbb{R}\\) which are not definable over \\(L\\). It's easy to see that substitutional quantification and objectual quantification must come apart in such a structure, even if we expand substitutional quantification to allow quantification over all definable elements. 

[Hugly and Sayward](https://www.jstor.org/stable/20117947) think arguments which aim to show that some elements of the reals must be unspecifiable proceed a little too quickly. 


