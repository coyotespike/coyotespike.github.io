---
layout: post
title: Two by Tufte
date: 2016-08-31 09:56
# Should be longer than 20 words, so it will appear as post summary
description: Edward Tufte is the Strunk & White of data visualization. My brief reviews of *Envisioning Information* and *The Visual Display of Quantitative Information*.
# tags will also be used as html meta keywords.
tags:
  - data science
  - data visualization

show_meta: true
comments: true
mathjax: true
gistembed: true
published: true
noindex: false
nofollow: false
---
<div id="table-of-contents">
<h2>Table of Contents</h2>
<div id="text-table-of-contents">
<ul>
<li><a href="#orgheadline4">1. <i>The Visual Display of Quantitative Information</i></a>
<ul>
<li><a href="#orgheadline1">1.1. The Lie Factor</a></li>
<li><a href="#orgheadline2">1.2. Simplicity and Ink Minimization</a></li>
<li><a href="#orgheadline9">1.3  A Theory of Data Graphics</a></li>
<li><a href="#orgheadline3">1.4. Concrete Recommendations</a></li>
</ul>
</li>
<li><a href="#orgheadline5">2. <i>Envisioning Information</i></a></li>
<li><a href="#orgheadline6">3. Details and Data</a></li>
</ul>
</div>
</div>

Having heard Edward Tufte's name many times over the last few years, I thought
I'd start with what seem to be his best books: *Envisioning Information* and *The
Visual Display of Quantitative Information*. Both are under 200 pages, and of
course have lots of pictures, though they reward leisurely reading.

## *The Visual Display of Quantitative Information*<a id="orgheadline4"></a>

Some reviews thought VDQI read like a textbook. While it does clearly enunciate
guiding principles - it consciously *teaches* - the book lacks the sterile and
disjointed tone of most textbooks. Rather, the prose and the graphics are a
paean to the marriage of simplicity and power.

In this the book strongly reminds me of *The Elements of Style*, with its "Omit
needless words" (a proverb that conspicuously practices what it preaches).

In the bad old days, graphics either misled, or barely instructed, the
stupid. 

> Graphics should be as intelligent and sophisticated as the companying text.

John Tukey, also a colleague of Richard Hamming, changed all that by
simply ignoring the dispiriting debate over *how not to mislead so much* and
instead demonstrating graphics' use as a tool for substantive data analysis.

> Multifunctioning graphic elements, if designed with care and subtlety, can
> effectively display complex, multivariate data.

Data visualization developed so late, and matured into respectability even
later, partly because it involves so many skills. "Graphical competence demands
three quite different skills: the substantive, statistical, and graphic."

Tufte's many elegant examples, and dryly humorous commentary on the poor
examples, illustrate a few fundamental and far-reaching principles.

### The Lie Factor<a id="orgheadline1"></a>

For one, the graphics must reflect the magnitude and ordering of the data. If
for political reasons the graphic exaggerates a drop in revenue, or an
increase in size over time of oil pollution, the graphic *lies*. Sure,
the barrels should get bigger - but not *that* much bigger!

Tufte derives a Lie Factor: the graphic's size increase divided by the actual
proportionate increase. Visualizations must show the actual relationships among
the data. A picture is not an excuse to make up proportions. With this idea in
hand, you'll see lies everywhere in graphics, attempting to slip in under your
critical radar.

### Simplicity and Ink Minimization<a id="orgheadline2"></a>

Tufte pursues his Strunkian theme through many charts:

> Maximise the data-ink ratio, within reason.

I was surprised at how much of the ink on a chart can be removed, making for a
simpler and clearer chart with an increase in understanding. 

For instance, on a bar chart, not only grid lines, but even the *bars* are
redundant! The bar chart becomes a white grid. Bar plots, which usually have a
"barrel and whiskers," become lines with dots to show the mass. The range-frame,
or even better, the dot-dash chart, replaces the usual scatter plot grid.

Another way of putting the same lesson is, "Forgo chartjunk." I will steal a
couple of quotations from *EI*, which continues the analysis of chartjunk. 

Some flavors of chartjunk are silly pictures designed to entertain at a simple
level: "Lurking behind chartjunk is contempt both for information and for the
audience."  

Some flavors of chartjunk are just design choices which overwhelm the main
information being imparted: For instance, "Dark grid lines are chartjunk."

### A Theory of Data Graphics<a id="orgheadline9"></a>
> The first part of a theory of data graphics is in place. The idea, as described
> in the previous three chapters, is that most of a graphic's ink should vary in
> response to data variation.

The presentation of data can be elegant and even beautiful. "How much can we
communicate with how little?" is the question. Words and numbers are sometimes
better than graphics - though sometimes words and numbers can be arranged so
that they *become* graphics.

> I want to reach that state of condensation of sensations which constitutes a picture. Matisse.

Presentation of data is really only data analysis, not data science. But because
data analysis is part of every data scientist's workflow, part of the
exploration phase, part of the creativity of noticing connections and coming up
with good questions, Tufte's work belongs in the head of every data
scientist. In addition, of course, the data scientist has to share her work, and
then she will need Tufte's book as well.

> For non-data-ink, less is more.
> For data-ink, less is a bore.

The ink-minimization principle forbids overwrought artistry and garish
colors. Personally, I think if we are not using beautiful colors then we must
pay more attention to hue, font, and lines. Very simple web pages and graphs can
look attractive, for reasons hard to express until you know how it was done.

The Lanyon Plus blog theme, for instance (like this website) is extremely
simple, not elegant, yet easy to read. I mean, let's not end up with Word or
Excel!

### Concrete Recommendations<a id="orgheadline3"></a>

Scattered throughout, and especially toward the end of the book, Tufte provides
some specific rules. These are not *hard* rules, mostly, but helpful suggestions.

> Maximise data density and the size of the data matrix, within reason.

We can use the Shrink Principle - most graphics lose nothing by being made
small - to fit many graphics at once. Over and over again, Tufte sings the
praises of *small multiples*. A small multiple is a progression of small charts
that can tell a story.

Some data does not benefit from graphic representation at all:

> One supertable is far better than a hundred little bar charts.

Because "graphical elegance is often found in simplicity of design and
complexity of data," he concludes:

> The only worse design than a pie chart is several of them&#x2026;pie charts should never be used.

On data/text integration:

> "Data graphics are paragraphs about data and should be treated as such."

That is, repeating or separating graphics and text leads to multiple or
redundant story lines, breaking the flow of your narrative.

Again I'll foreshadow EI with a quotation:

> *Comparisons must be enforced within the scope of the eyespan*, a fundamental
> point occasionally forgotten in practice.

Tuft also deals with design principles such as line weight and lettering,
proportion and scale, and labeling. Most charts should be wider than tall, so
the story can unfold, unless the shape of the data dictates the shape of the
graphic.

Design is choice, he enjoins us, and we should choose so as to reveal the complex.

## *Envisioning Information*<a id="orgheadline5"></a>

If VQDI was about accuracy and simplicity, EI is more about complexity. How can
we represent many dimensions - all the aspects of the problem which matter - on
two-dimensional paper? How much information per square inch, as it were, can we
communicate?

> Escaping this flatland [of paper] and enriching the density of data displays are
> the essential tasks of information design. Such escapes grow more difficult as
> ties of data to our familiar three-space world weaken (with more abstract
> measures) and as the number of dimensions increases (with more complex
> data). Still, all the history of information displays and statistical graphics —
> indeed of any communication device—isentirely a progress of methods for
> enhancing density, complexity, dimensionality, and even sometimes beauty. Some
> of these methods, identified and described in the chapters that follow, include
> micro/macro readings of detail and panorama, layering and separation of data,
> multiplying of images, color, and narratives of space and time.

Surveying the historical landscape, sometimes re-using graphic examples from
VDQI, Tufte finds certain principles which unite the disparate array of examples.

> Note all the different techniques for displaying sunspots during 380 years of
> data analysis — from Galileo's first precious observation of the solar disk, to
> small multiple images, to dimensionality and data compression, and finally to
> micro/macro displays combining pattern and detail, average and variation. 
> 
> Exactly the same design strategies are found, again and again, in the work of
> those faced with a flood of data and images, as they scramble to reveal, within
> the cramped limits of flatland, their detailed and complex information. These
> design strategies are surprisingly widespread, albeit little appreciated, and
> occur quite independently of the content of the data.

Tufte builds on the argument he began in VDQI against over-simplification. He
*needs* to make this argument, because the universal tendency is to assume a
high-information-density chart will inevitably be hard to read.

> Now and then it is claimed that vacant space is "friendly" (anthropomorphizing
> an inherently murky idea) but /it is not how much empty space there is, but
> rather how it is used. It is not how much information there is, but rather how
> effectively it is arranged./ (emphasis in original)

The elegance of [John Tukey's leaf-and-stem plot ](http://ilyabirman.net/meanwhile/all/tufte-mystery/) repeatedly excites Tufte's
admiration: a macro chart made up of micro data, with the micro made still finer
by using the volcanos' height in digits to make up the bar chart.

In VQDI, I got the impression that Tufte was opposed to all color. Here he
corrects that misapprehension. Color may be used to label, to measure, to
imitate reality, and to decorate. The problem is using color well: "Color itself
is subtle and exacting."

> *Clutter and confusion are failures of design, not attributes of information.*
> Often the less complex and less subtle the line, the more ambiguous and less
> interesting is the reading.

## Details and Data<a id="orgheadline6"></a>

At the end of the day, the graphic should reveal as much of reality as possible.

> What matters — inevitably, unrelentingly — is the proper relationship among
> information layers. These visual relationships must be in relevant proportion
> and in harmony to the substance of the ideas, evidence, and data conveyed.

"Measured assessments of variability are at the heart of quantitative
reasoning," Tufte writes, and we must design graphics that aid and reveal
quantitative reasoning with respect for our audience and passion for the truths
we seek.

> "God is in the details," said Mies van der Rohe, capturing the essential quality
> of micro/macro performances.

As Andrew Gelman likes to say, "God is in every leaf of every tree," explaining
that this means the simplest problem can implicate techniques at the limits of
human knowledge.

With these two masterworks, Edward Tufte shows how to combine simplicity and
elegance with multivariate complexity through detailed design decisions. Instant
classics upon publication, they'll retain their freshness for many decades to
come.
