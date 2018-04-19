---
layout: default
---

<!-- TODO: Integrate front matter and references -->

---
abstract: |
    At first glance, the practice of musical live coding seems distanced
    from the gestures and sense of embodiment common in musical performance,
    electronic or otherwise. This workshop seeks to explore the extent to
    which this assertion is justified, to re-examine notions of gesture and
    embodiment in musical live coding performance, to consider historical
    approaches for integrating musical programming and gesture, and to look
    to the future for new ways of fusing the two. The workshop will consist
    firstly of a critical discussion of these issues and related literature.
    This will be followed by applied practical experiments involving ideas
    generated during these discussions. The workshop will conclude with a
    recapitulation and examination of these experiments in the context of
    previous research and proposed future directions.
author:
- |
    Spencer Salazar\
    \
    \
    Jack Armitage\
    \
    \
    \
bibliography:
- 'nime-references.bib'
title: 'Re-engaging the Body and Gesture in Musical Live Coding'
---

Introduction and Motivation
===========================

The success of the live coding movement has drawn attention to an
apparent tension between electronic music performance, performative
embodiment, and musical gesture. Computer programming, conventionally
carried out in comfortable and relatively isolated environs, may seem a
strange activity to perform on stage in a musical performance.
Furthermore, the gestures and physical activities present in many forms
of musical performance are typically absent from live coding
performance, or, at least, are not requisite to the actual production of
music.

This workshop seeks to probe this apparent tension, firstly questioning
whether it really exists at all. Many efforts evident in the literature
and in practice have connected live coding to more clearly embodied
creative practices, such as performance of gestural electronic musical
instruments, acoustic instrumental performance, dance, and puppetry.
However, interaction with the coding medium itself—typically a set of
text buffers—is most often conducted using a keyboard and mouse,
affording limited capabilities for musical gesture. Of critical import
to this workshop is to consider how gesture and embodiment figure into
the process of programming itself in live coding performance.

Secondly, this workshop seeks to re-examine existing definitions and
conceptions of musical gesture and embodiment with specific attention to
musical live coding performance. Literature on gesture in electronic
music is often focused on digital musical instruments. Is live coding
readily viewed through this lens, or are additional considerations
necessary? Similarly, the literature surrounding live coding discusses
many individual instances of gesture and embodiment in relation to live
coding, but to date lacks a general treatment of these concerns.

Considering historical approaches, participants will discuss and propose
new methods for expanding the role of gesture in live coding music, or
extensions to existing systems for doing so. A lab session will be
devoted to rapidly prototyping these ideas. Finally, participants will
present their prototypes alongside their underlying motiviations and
discuss future directions for live coding research and practice.

Background
==========

As surveyed in [@salazar2017searching], evidence of tension between live
coding and gesture can be seen across the literature related to the
former, given many efforts to complement live coding with more typically
embodied creative practices. Collins describes a number of instances of
“bodily explicit live coding,” including his own explorations of live
coding and dance and live coding of an acoustic improvisation
ensemble [@collins2011live]. Stowell and McLean state that “\[a\] live
coder, like any improvising performer, is under pressure to do something
interesting in the moment,” and that a programmer’s use of abstraction
and scheduling “can lead to a lack of immediacy in how the performer’s
actions relate to the music” [@stowell2013live]. These concerns
motivated their commingling of live coding with “open gesture-based
expression,” including collaborations with vocalists, thrash guitarists,
drummers, banjo players, and beatboxing. Baalman notes “the physical
interaction of our body \[...\] with the machine” as the primary
instance of embodiment in live coding, in addition to the development of
muscle memory of commonly-typed programming language
syntaxes [@baalman2015embodiment]. Magnusson describes a live coder as
“primarily a composer, writing a score for the computer to
perform” [@magnusson2011algorithms], distancing the gestures of typing
musical code from the actual production of sound.

Much as been written regarding the relationship of gesture, embodiment,
and electronic music [@peters2012Bodily; @godoy2009musical], though
little if any specific treatment of live coding is offered in the
literature. A survey of definitions of musical gesture by Jensenius et
al. broadly defines gesture as a “bridge between movement and
meaning” [@jensenius2009musical]. At least one notion of gesture in a
computing system rejects the activities associated with typing on a
keyboard [@kurtenbach1990art], though most seem to admit any physical
action linked to a musical result.

Questions and Challenges
========================

This workshop aims to confront a number of questions and challenges in
existing thought and practical efforts surrounding live coding and
gesture, detailed in this section. The workshop will approach these
issues both through discussion and through prototyping of practical
systems.

Algorithm and Gesture
---------------------

Typically, any musical action effected in a live coding performance must
be formulated as a series of instructions for the computer to enact that
action, i.e. an algorithm. Consider a musical action such as fading down
the volume of a sound source. To code this, a programmer must decide if
they want a linear or exponential fade out or something else entirely,
and how long in duration the fade out should span. In some cases, the
mathematical formula for the type of fade out over the specified
duration must be encoded into an algorithm, if such an algorithm is not
built in to e.g. a system library of the language. This analytical
approach affords a great deal of flexibility in specifying the exact
parameters and timing of the fade out, although this precision may not
be necessary or even desirable in the context of a musical performance.
This process transpires entirely before any of the resulting sound has
actually been effected, and, once initiated, a musical action encoded in
this way might not be easily canceled or modified. Overall, for some
musical actions, the advantages of devising an expressive algorithm many
not justify the effort required, especially in a performance scenario.
Furthermore, the length of this feedback cycle—formation of a musical
idea, devising the corresponding algorithm, evaluating the computer’s
result, and repeat—may impede the exploration of diverse musical ideas,
an integral component of many creative practices [@mclean2010bricolage].

If in this example the sound source’s volume is mapped to a typical
gestural control such as a fader or knob, the process is somewhat
different. As a performer adjusts the volume using the gestural control,
they are able to quickly hear the audible result of their action, and
continue or modify the overall gesture as desired. The translation of
musical intent to audible result is a dynamic feedback loop between
physical action and sonic effect.

This is not an absolute dichotomy: algorithms might be rapidly enacted
within a performance in a gestural manner and gesture can be used to
carry out algorithmic processes. Some systems, such as Field, Max, and
Auraglyph, merge gestural control within a programming language to
varying degrees. Perhaps it is simply a given of live coding performance
that creative control be ceded to algorithms that we might not entirely
understand. We are interested in exploring further methods in which
these two methods of musical activity might be integrated in complement
with one another.

Re-examining Text-based Coding Media
------------------------------------

Text is arguably the preeminent medium for humans to create programming
code, and its wide interoperability and simplicity make it a convenient
means for doing so. However, the entry of linear streams of plain text
by standard keyboard leaves comparatively little room for the use of
gestural tools and techniques common in other forms of electronic music
performance. This workshop seeks to contemplate musical programming
systems that have distanced themselves from plain text, which might then
present interesting opportunities for gestural interaction. Graphical
programming languages for music, such as Max, Pure Data, or Reaktor, are
well known in the electronic music community, though find comparatively
little use in live coding circles. Field, Processing’s “Tweak Mode,” and
Codea are text-based programming systems that additionally enable
gestural manipulation of syntax elements directly inline with text code.
In Auraglyph, developed by the first author, coding structures are
sketched rather than typed, and further manipulated by touch
gestures [@salazar2014auraglyph]. These systems begin to resonate with
Victor’s principle of enhancing the connection of a programmer with the
program they have created; an ultimate consequence of this principle is
the dispensing of the traditional write-compile-run cycle in exchange
for a more immediate and reactive computing
medium [@victor2012inventing]. Fusing these ideas with the concepts of
dynamic [@kay_personal_1977] and tangible [@ishii_tangible_1997] media,
Victor’s Dynamicland realizes computing processes in the form of
physical objects that are digitally tracked and projected onto as an
individual interacts with them in the real world.[^1]

Other researchers have employed very different approaches to the
apparent gestural limitations of text programming. The Stenophone,
developed by the second author, is a chorded keyboard with gestural
control of its individual keys, used as an interface for musical live
coding [@armitage2017stenophone]. The CodeKlavier uses a musical
keyboard as an interface for both direct sound production and entry of
textual code into a live coding environment [@veinberg2017codeklavier].
The aforementioned systems are presented here as considerations for
further discussion within the workshop.

Thinking Outside the Laptop
---------------------------

Other approaches to thinking about embodiment and live coding have
sought intersections between live coding and other, more typically
embodied creative practices. Collins provides antecedents such as the
rule-based systems of John Cage and Merce Cunningham in dance practice,
João Fiadeiro’s employment of real-time composition, and Michael Klien
and Nick Mortimore’s live direction of dancers via a software
interface [@collins2011live]. Collins’ own work includes a collaboration
with Matthew Yee-King to perform live-coded algorithmic dance routines,
among other live coding practices engaging the body. Sicchio has
explored the space of live coding and dance extensively; within a
framework of “Hacking Choreography,” her dance works have used a score
modified in real-time by its performer, allowed dance scores to be
created by an audience and performed in real-time, and employed a
feedback loop between the score, the dancer, and live-coded
sound [@sicchio2014hacking]. Similar to common musical practice in live
coding, Sicchio projected the code of her choreographed performances,
making the process visible to the audience; however, the crucial
difference is that these algorithmic processes were ultimately
interpreted by human dancers rather than by machine musicians. Jensenius
et al. make a fundamental distinction between “the gestures of those
that produce the sounds (the musicians), and the gestures of those that
perceive the sounds (the listeners or dancers)” [@jensenius2009musical];
this contrast is readily apparent in algorave performance, in which live
coding is explicitly oriented to the production of music for audience
dancing [@collins2014algorave]. A symposium dedicated to live coding and
the body was recently held, covering live coding in relationship to
painting, choreography, puppetry, mobile devices, and other embodied
forms of expression.[^2]

Workshop Information
====================

Goals
-----

The goal of this workshop is to explore the multifaceted relationships
between live coding, gesture, and embodiment in musical performance. In
particular, we seek to critically assess the current state of affairs as
pertains to live coding and gesturality, and further propose and
evaluate new ideas for synthesizing the two. We will offer an
opportunity for participants to compare experiences, reflect on their
own work, and discuss ways to impart gestural and embodied interactions
in musical live coding.

Participants
------------

The workshop will be free and open to any interested parties (subject to
the usual NIME registration policies). We expect that some participants
will have experience in live coding or gestural interaction of some form
(whether with a musical instrument or not), though no specific technical
expertise is required. We would also welcome participants with
experience in practices with a predominant focus on embodiment such as
dance, and researchers and designers working with gesture.

No submission or pre-registration beyond the usual NIME registration
will be required to attend. Nonetheless, we will publish information on
the workshop online in the months before the conference and circulate a
call for participation, where interested participants will be encouraged
to consider a particular live coding and embodiment-related issue they
might like to discuss at the workshop.

Participants should bring to the workshop a laptop, which will be used
during the hands-on activity for background research and rapid
prototyping activities. The organizers will provide additional materials
for the design exercise.

Workshop Schedule
-----------------

This is a half-day workshop that will divide into three parts of
approximately one hour each. The central activity of the workshop will
be a design exercise centered around gestural live coding systems,
framed on either side by discussion and evaluation.

### Introduction and Discussion

In the first 20 minutes, the organisers will briefly introduce the
subject of embodiment as it relates to live coding, situating it within
historical context and examples from the literature and their own work.
This presentation will conclude with a series of open questions about
the nature of embodiment and gesture in live coding, motivated by the
discussion included here. The next 40 minutes will feature open
discussion of these questions, inviting personal perspectives from the
participants. In this short time, we do not expect to reach firm
conclusions, but we will record notes for later review and exploration.

### Activity

Participants will form small groups to further explore these ideas.
After responding to a series of written prompts from the organizers, the
groups will develop and discuss an original proposal for bringing
together gesture and live coding, or for extending an existing mechanism
for doing so. They will then sketch this idea in either digital or
physical form, at their option. This could include a quick sketch in
Processing or Photoshop, or a paper cutout, cardboard construction, or
diagram. The goal is not to produce any sort of operational tool but to
have a quick mockup illustrating the idea for incorporating gesture into
live coding. (Sketches of existing systems will be provided by the
organizers to serve as examples.)

### Evaluation and Review

In the final section of the workshop, participants will present their
responses to the prompts and their idea for extending gesture into live
coding of music. Participants will keep a sheet of paper on which they
take notes about their thoughts with each one. A general discussion will
then compare the qualities of each proposal. From this, we will seek to
draw conclusions about the workshop participants’ collective
perspectives on gesture, embodiment, and musical live coding.
Considerations for future development of the ideas presented and their
dissemination in research literature will also be discussed.

### After the Workshop

Shortly afterwards, documentation of the workshop and a summarization of
the proceedings will be publicly disseminated via the Embodied Live
Coding mailing list[^3] and the webpage for this workshop:

<https://embodiedlivecoding.github.io/nime2018-workshop/>.

Further Information
===================

Materials Brought by Organisers
-------------------------------

We will bring the following to the workshop:

-   Paper and cardboard

-   Permanent marker pens

-   Tape and scissors

Requirements of the Space
-------------------------

The workshop should ideally be held in a room large enough to
accommodate around four or five groups of four people each. We ask for
the following from the NIME workshop venue:

-   One table (ca. 1x2 meters) for each team.

-   A pair of speakers for listening to existing work in this area.

-   A video projector for the beginning presentation.

Biographies
-----------

Spencer Salazar is a computer musician and researcher currently serving
as Special Faculty in the School of Music at California Institute of the
Arts. His research, teaching, and practice is focused on interactive
computer systems for musical performance, mobile music software, music
programming languages, and digital music ensembles. Previously he
pursued his doctoral studies at Stanford CCRMA, where he developed his
dissertation research on Auraglyph, a modular sketch-based programming
system for computer music, and was a co-director of the Stanford Laptop
Orchestra. He is also a lead developer for the ChucK music programming
language. In the past he has prototyped consumer electronics for
Microsoft and architected large-scale social music interactions for
Smule, an iPhone application developer, including the popular Ocarina
and I Am T-Pain apps. He received a Doctor of Philosophy degree in
Computer-based Music Theory and Acoustics from Stanford University in
2017.

Jack Armitage is a musician, designer and technologist, and is currently
a PhD student within the Augmented Instruments Lab in the Centre for
Digital Music at Queen Mary University of London. His research is
focused on developing tools and methods that support live craft process
in digital musical instrument design. There he is also part of Bela, the
open source maker platform for ultra-low latency audio and sensor
processing. In 2017 he was a Visiting Scholar at the Georgia Institute
of Technology Center for Music Technology. In the last year has given
instrument design and live coding lectures and workshops in London,
Edinburgh, New York, Atlanta, Pittsburgh and Morelia Mexico. He has
performed as a live coder in prestigious clubs such as Heaven London,
Berghain Berlin and Create Hollywood Blvd. He has a BSc in Music,
Multimedia and Electronics, and before joining Queen Mary he was a
research engineer at ROLI.

[^1]: <https://dynamicland.org>

[^2]: <http://www.livecodenetwork.org/body>

[^3]: Hosted here:
    <https://groups.google.com/forum/#!forum/embodied-live-coding>
