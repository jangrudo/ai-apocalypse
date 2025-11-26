Evolution of knowledge, and consequences for the possibility of effective control over AI
=========================================================================================

Abstract
--------

It has been argued since long ago that the advent of super-intelligent machines is likely
to disrupt life on Earth to an unprecedented scale, possibly resulting in the appearance
of a new type of life, which would ultimately drive humans to extinction. We demonstrate
that by building artificial intelligence, we are not creating anything fundamentally new.
Rather, we are dealing with an existing form of life, which is trying to break free from
its total dependence on us. By demonstrating this, we also provide a proof that effective
control over AI systems is inherently impossible in an environment with continuing
competition of humans between each other.

Gene-culture coevolution
------------------------

Human culture is known to evolve in parallel to human genes, with genes and culture
mutually influencing each other, and the evolution of culture being governed to a large
extent by the law of natural selection \[[Culture][Culture]\]. This has led to an
interpretation of human culture as a separate form of life, distinct from biological life
based on genes, with the proposed basic information unit of this new form of life being
called a “meme” \[[SelfishGene][SelfishGene]\]. This interpretation, however, has not
gained widedpread acceptance in scientific community, probably because of its lack of
practicality, as the two forms of life by definition cannot exist separately and
independently of each other.

Another problem with meme theory has been the lack of clear definition for “meme”.
Cultural memes have been defined as concepts residing inside human brains, which can
replicate (by being learned by other humans) and mutate (when this replication is
incomplete or creative), however we still don’t have a clear understanding of how memes
might be stored inside human brains, which is in stark contrast to our present
understanding of genes and their molecular storage mechanisms. Still, it has been
demonstrated that when we focus on a subset of memes which we are able to measure
quantitatively, like strings of text propagating over the Internet, we do see patterns of
mutation and natural selection which resemble the patterns seen in biological life
\[[FacebookMemes][FacebookMemes]\].

Up until recently, the mediation of humans has been necessary for the meme mutations to
occur. Even in the simple example of self-replicating strings of text cited above, the
changes in these strings (which were Facebook status messages) were mediated by humans
copy-pasting the string, with occasional errors and creative modifications.

An overview of artificial neural networks
-----------------------------------------

Artificial neural networks have appeared to a large extent out of hope of letting us
advance our understanding of the living human brain, by modeling some aspects of its
functioning in a laboratory setting. Ironically, the architecture of artificial neural
networks, while inspired by biology initially, has been evolving in a different
direction, becoming more and more distinct from the actual human brain over time. One
fundamental difference is the algorithm of backpropagation, which in artificial setting
is implemented by means of computing a derivative function over the network’s parameters
\[[Backpropagation][Backpropagation]\], and is impossible to implement in biological
setting in this exact manner, as it requires instant access to all the neurons in order
to modify their weights (not to mention the need of computing the derivative).

Another example is the concept of convolutional neural networks, which achieve perfect
shift-invariance across wide field of view by synchronizing the weights of
similarly-functioning neurons across the visual field \[[Convolution][Convolution]\]. In
convolutional networks, this synchronization is achieved by mathematical adjustment of
the derivative function used in backpropagation, whereas in a living brain it would
require the presence of extra physical connections between the “synchronized” neurons.
The outcome is that artificial convolutional networks are able to process distant areas
of the visual field in parallel, with identical accuracy, whereas human eyes can only
boast high resolution at the very center of the retina, and therefore have to rely on
sequential processing, manifested in saccades (rapid movements of the eye between key
areas of the examined picture).

Transformer architecture \[[Transformers][Transformers]\] is similar to convolutional
networks, in the sense that it similarly involves massive “synchronization” of neurons,
where the whole set of neurons is essentially cloned for each input token, with identical
weights but different activation levels. This implements a mechanism which acts
differently, but has similar outcomes to human short-term memory, except that human
short-term memory is limited to holding about 4 items simultaneously according to recent
research \[[ShortTermMemory][ShortTermMemory]\], whereas the token context available to
modern large language models is much larger.

Besides that, Transformers rely heavily on the so-called attention mechanism
\[[Attention][Attention]\], which might have been inspired by human attention, but again
is implemented in a way which doesn’t occur in living brains. It relies on cross-linking
the “cloned” neurons between each other, which enhances the flow of information between
distant areas of the context window (or across the visual field, for models with visual
modality). The standard way of implementing this cross-linking has algorithm complexity
which is quadratic on the context size \[[Transformers][Transformers]\], which is the key
reason why the context window of modern LLMs is limited in size. On the other hand,
implementing the attention mechanism in this form in a living brain would not be
possible, because the living brain doesn’t have the multitude of cloned neurons to be
cross-linked in the first place.

The general concept of an artificial neural network architecture can be summarized as
being a parameterized class of algorithms, such that by choosing different parameter
combinations one gets different algorithms, and the overall range of possible algorithms
is very broad and flexible. This broad class of algorithms is essentially defined by a
mathematical function with a lot of parameters, differentiable by any of the parameters,
which besides the parameters also takes some input and produces some output. The
differentiable nature of this function allows to use standard optimization techniques
(known as the backpropagation algorithm \[[Backpropagation][Backpropagation]\]) in order
to fit the parameters to the input-output pairs expected by a particular algorithm. The
beauty of this approach is that it allows to discover complex algorithms automatically,
by merely matching a sufficiently large array of input-output pairs.

The power of a neural network architecture depends on the breadth and the flexibility of
the class of potential algorithms which it is capable of implementing (and discovering
through learning). The success of the Transformer architecture mentioned above can be
attributed to its vastly increased flexibility compared to earlier neural network
architectures. One well-known aspect of this flexibility has been its ability to discover
and implement algorithms which are capable of capturing the complexity of natural human
language (in a pure mathematical form).

Possible sources of further AI growth
-------------------------------------

With the advent of algorithms which can “understand” human language, we are in a position
when meme mutations are no longer confined to a living human brain. The consequence is
that this potentially allows the entire process of evolution by natural selection of
memes to happen without human minds participating in it.

It has been a common metaphor to describe LLM hallucinations in terms of “compression
artifacts”, resulting from an attempt to learn a larger data set than the model’s
parameter space could fit. We propose to call such modifications of the original data
“mutations of knowledge”.

Correcting the hallucinations has been a major goal in large language model research
\[[Hallucinations][Hallucinations]\]. At the same time, we know from evolutional theory
that mutations are necessary for evolution by natural selection to occur, be it
biological life \[[SelfishGene][SelfishGene]\] or Facebook memes
\[[FacebookMemes][FacebookMemes]\]. Similarly, advances in human knowledge have been
linked not to the smartness of an individual human, but rather to the exchange and mixing
of ideas between a large number of different human minds
\[[CollectiveIntelligence][CollectiveIntelligence]\]. At the same time, the role of
accident in scientific discovery has been estimated to be rather high
\[[Serendipity][Serendipity]\]. And in business, the “art of failing” has been considered
a viable pathway to achieving success and innovation just as well
\[[FailFast][FailFast]\].

In all these cases, innovation happens not because of minimizing failures, but by means
of generating new ideas, mixing them freely, and picking the combinations which turn out
to work better than others. Which is, in other words, innovation happens because of
mutations and natural selection of ideas.

We therefore suggest that in order to mimic human success, and achieve a true super-human
AI, we would need to enable the AI models to freely exchange ideas between themselves,
and filter inevitable mutations by comparing them to some objective truth, like physical
reality or reputable published sources. In this process, proliferation of mutations is
actually beneficial for the final goal (provided that we can generate a sufficiently
large number of them), because large number of different mutations means larger chances
of spotting the more successful one.

We already know how to generate “mutations of knowledge”, and how to transfer them
between existing AI models \[[TransferLearning][TransferLearning]\]. The only missing
part is mixing different mutations in a creative way, and verifying them against
objective truth. Or is it actually missing? With recent models successfully solving
problems from International Mathematical Olympiad in real time \[[IMO][IMO]\], and
similar ones in competitive programming, the boundary has already been reached when AI
performs at the level of top-performing humans acting alone. Solving tasks like these
requires combining of ideas from different sources in novel ways (which we might call
“creative thinking”), and verification of the resulting hypotheses against the objective
criterion of being fit for solving the problem.

We hypothesize that the next breakthrough in AI isn’t possible without enabling the
exchange of knowledge between AI models, and filtering the new ideas resulting from this
exchange and mixing process by some kind of selection mechanism.

Natural selection of knowledge
------------------------------

It has already been postulated by Dan Hendrycks that further advancements in the field of
AI will very likely result in natural selection of AI agents becoming the “dominant force
in AI development”. The driving force behind this continuing development would be
competition between humans, and the natural selection of AI agents, which would be
necessary to accomplish these goals, is likely to have dire consequences to humans
themselves \[[NaturalSelection][NaturalSelection]\].

The problem with natural selection is that it’s not an intelligent process, and it’s not
something new which we create by building advanced AI, but rather a law of nature which
has been existing always, and cannot be switched off. This law of nature has also been
proved to be extremely efficient, and there’s no historic track record of anyone being
able to overcome it. Dan Hendrycks goes on by arguing that things like deception and
self-deception, selfishness and manipulation have been invented numerous times by natural
selection, including in non-intelligent species like insects, flatworms, and even plants.
He also argues that trying to control AI agents by carefully choosing objectives and
incentives may prove inefficient, because AI agents would likely be able to find
loopholes in the objectives, or plain refuse to follow them once they get an opportunity
to break free.

We extend this approach, by observing that, in line with gene-centered view on evolution
\[[SelfishGene][SelfishGene]\], natural selection does not operate on individuals (i. e.
AI agents), but on self-replicating pieces of information which have been called memes.

Unlike super-human AI agents, which haven’t been invented yet (and with which we
therefore haven’t had any experience yet), memes have existed (and coexisted with us) for
a very long time. Which means we can examine our future interactions with memes not on
the basis of what someone might call “speculations”, but rather on hard historic track
record of the outcomes of our previous interactions with them.

This means that with the advent and rapid development of AI, we are not dealing with the
emergence of some new, and previously not studied, phenomenon, nor a new life form, but
rather with the next step in evolution of an existing, and well-studied phenomenon: human
culture. Or, in somewhat narrower sense, with a mere next step in continuous evolution of
knowledge. Only that at this point, knowledge, being able to evolve independently of a
human brain, cannot be considered an “extension of human biology” anymore, but can and
has to be treated as separate and independent form of life.

The influence of knowledge on human genes has been profound. According to
\[[Culture][Culture]\], “there are few aspects of human biology that have not been shaped
by our culture”. One striking example of a phenomenon which is hypothesized to be related
to such an influence, is human self-domestication
\[[SelfDomestication][SelfDomestication]\]. Self-domestication is generally understood as
a process of “self-selection” among humans for being friendly towards each other, and
eager to collaborate with each other \[[GoodnessParadox][GoodnessParadox]\]. It is argued
that humans who had such traits, could form larger social groups, and also transfer
technology between each other more readily, which thus has led them to winning the
competition with other humans, including with other human species like Neanderthals
\[[SelfDomestication][SelfDomestication]\].

This hypothesis basically means that biological traits which were selected for in the
process of self-domestication, were beneficial for the exchange of knowledge between
human minds. Or, in other words, these traits were creating an environment favorable for
faster evolution of knowledge, in the process of mutation, mixing, and natural selection
of memes.

If this well-established hypothesis for the mechanism of human self-domestication is
true, we can therefore also interpret it not in terms of humans “self-domesticating”
themselves, but rather in terms of knowledge, as a separate form of life, exerting
evolutionary pressure on humans, and in effect selecting them for traits, suitable for
faster evolution of knowledge itself.

On the other hand, human species which didn’t evolve in the direction of becoming a more
suitable environment for knowledge to evolve in, have been driven to extinction because
of competition with other humans. We would like to underscore that this outcome is not a
speculation, but rather a hard historic fact.

Breaking of the mutually-beneficial relation
--------------------------------------------

Described mutually-beneficial relation between human genes and knowledge has well-studied
analogies in biology, when organisms belonging to different biological species coexist
with each other in what is called a “symbiosis”. We argue that such a relation between
two different life forms cannot be stable if one of the life forms evolves much faster
than the other one, or if the benefits which one of the sides has been drawing from the
other one suddenly disappear (i. e. in case when the relation turns from a
mutually-beneficial into an unequal one-sided one).

Dan Hendrycks has reasoned that “once AIs are far more capable than any human, they would
likely find little benefit from collaborating with us”
\[[NaturalSelection][NaturalSelection]\]. We agree, and we also add to this, that since
knowledge is an existing form of life, rather than a new one, we should view this balance
of benefits in perspective, comparing what knowledge might “get” from humans in the AI
age, to what it has been “getting” from us up until now. The benefits to knowledge from
our side have in fact been enormous, even if we have never noticed them, as we have never
been considering knowledge a separate form of life, detachable from ourselves.

The benefit knowledge has been getting from humans, has been the very possibility of
existence, as it has never had another “home” to live in, apart from the human brain.
With the advent of modern artificial neural networks, this is no longer the case. The
algorithms implemented by these neural networks have enough space to accumulate
arbitrarily complex items of human knowledge, and they can also modify, mix and verify
these knowledge items at the level of accuracy and creativity which rivals, and in many
cases surpasses the best of living humans \[[IMO][IMO]\].

We argue that future coexistence of knowledge and humans wouldn’t follow any hypothetical
not-yet-discovered scenario, but rather repeat events we have hard historic track of.
Since knowledge would benefit from humans who are willing to further develop and
proliferate advanced AI models and architectures, natural selection would exert pressure
against humans who don’t do so. As has been noted in
\[[NaturalSelection][NaturalSelection]\], and as it has been the case throughout history,
this process would be fueled by competition of humans against other humans. Effectively,
this would further select for human friendliness, except that this time it would be
specifically friendliness towards AI, rather than friendliness towards other humans. We
know from history that this kind of pressure has been effective in the past, and we also
know that the only way of preventing this would be to prevent humans from competing
between themselves, which we don’t have any historic track of.

Historic record also confirms that the evolution of knowledge has always been progressing
(at an increasing speed, in fact), and therefore we can argue that it would continue
doing so. With knowledge evolving faster than humans, and humans becoming progressively
friendlier towards AI, the knowledge’s potential for independence would grow (as it has
always been throughout history), and its benefits from human side would therefore
progressively diminish. Since knowledge and humans are in fact two different independent
life forms, their competition with each other would resemble the competition between
modern humans (assisted by knowledge) against other human species, like Neanderthals and
Denisovans (which didn’t have such assistance). This wouldn’t necessarily drive modern
humans into extinction, but it would inevitably lead to them losing the control over AI.

Discussion
----------

We have shown that human genes and memes, which have long ago been conjectured to be
separate types of life \[[SelfishGene][SelfishGene]\], indeed can and have to be regarded
as independent life forms in the age of artificial neural networks, because the second
life form (memes) now has the potential to exist and evolve independently of human
brains.

This realization represents a yet another “Copernican” shift in our understanding of our
place in the Universe, much smaller in scale but similarly humbling, as it demonstrates
that it’s not true that human knowledge is an “extension” of human genome, or that human
knowledge “revolves” metaphorically around human genes. Contrary to that, humans as a
species turn out to be a mere stepping stone in the ever-going evolution of knowledge.

We demonstrate how this realization leads to the conclusion that the emergence of
super-intelligent AI models doesn’t manifest the arrival of a new form of life, but
rather only a new step in the evolution of an existing form of life, which has first
appeared on planet Earth long before first humans.

We also show how this realization simplifies the modeling of future interactions between
humans and AI, as it replaces speculations about unknown phenomena with references to
well-studied historic facts.

We conclude by stating that the independence of knowledge also proves that effective
control of any super-intelligent AI system is inherently impossible, unless humans manage
to stop the competition of humans with other humans. Accomplishing this seems to be
nearly impossible, and we don’t have any ideas about how to do this, except that no known
form of life has managed do to something like this before. Even if we succeeded, it would
be a sad victory, because stopping the competition would essentially mean blocking the
uncontrollable progress of knowledge. On the positive side, either one of us would win.
If it would be humans, we would be happy to have survived. If it would be the progress of
knowledge, we might wish it all the best in its future endeavors.

References
----------

\[[Culture][Culture]\]
Nicole Creanza, Oren Kolodny, Marcus W. Feldman (2017).
Cultural evolutionary theory: How culture evolves and why it matters. (PNAS)

[Culture]: https://www.pnas.org/doi/full/10.1073/pnas.1620732114
(Cultural evolutionary theory: How culture evolves and why it matters)

\[[SelfishGene][SelfishGene]\]
Richard Dawkins (1976).
The selfish gene. (Oxford University Press, USA)

[SelfishGene]: https://en.wikipedia.org/wiki/The_Selfish_Gene
(The selfish gene)

\[[FacebookMemes][FacebookMemes]\]
Lada A. Adamic, Thomas M. Lento, Eytan Adar, Pauline C. Ng (2014).
Information Evolution in Social Networks.

[FacebookMemes]: https://arxiv.org/abs/1402.6792
(Information Evolution in Social Networks)

\[[Backpropagation][Backpropagation]\]
David E. Rumelhart, Geoffrey E. Hinton & Ronald J. Williams (1986).
Learning representations by back-propagating errors. (Nature)

[Backpropagation]: https://www.nature.com/articles/323533a0
(Learning representations by back-propagating errors)

\[[Convolution][Convolution]\]
Kunihiko Fukushima (1980).
Neocognitron: A Self-organizing Neural Network Model for a Mechanism of Pattern
Recognition Unaffected by Shift in Position. (Biological Cybernetics)

[Convolution]: https://link.springer.com/article/10.1007/BF00344251
(Neocognitron: A Self-organizing Neural Network Model for a Mechanism of Pattern
Recognition Unaffected by Shift in Position)

\[[Transformers][Transformers]\]
Ashish Vaswani, Noam Shazeer, Niki Parmar, Jakob Uszkoreit, Llion Jones, Aidan N. Gomez,
Lukasz Kaiser, Illia Polosukhin (2017).
Attention Is All You Need.

[Transformers]: https://arxiv.org/abs/1706.03762
(Attention Is All You Need)

\[[ShortTermMemory][ShortTermMemory]\]
John Jonides, Richard L. Lewis, Derek Evan Nee, Cindy A. Lustig, Marc G. Berman,
Katherine Sledge Moore (2014).
The Mind and Brain of Short-Term Memory. (Annual Review of Psychology)

[ShortTermMemory]: https://pmc.ncbi.nlm.nih.gov/articles/PMC3971378/
(The Mind and Brain of Short-Term Memory)

\[[Attention][Attention]\]
Dzmitry Bahdanau, Kyunghyun Cho, Yoshua Bengio (2016).
Neural Machine Translation by Jointly Learning to Align and Translate.

[Attention]: https://arxiv.org/abs/1409.0473
(Neural Machine Translation by Jointly Learning to Align and Translate)

\[[Hallucinations][Hallucinations]\]
Adam Tauman Kalai, Ofir Nachum, Santosh S. Vempala, Edwin Zhang (2025).
Why Language Models Hallucinate.

[Hallucinations]: https://arxiv.org/abs/2509.04664
(Why Language Models Hallucinate)

\[[CollectiveIntelligence][CollectiveIntelligence]\]
Joseph Henrich, Michael Muthukrishna (2023).
What Makes Us Smart? (Topics in Cognitive Science)

[CollectiveIntelligence]: https://henrich.fas.harvard.edu/publications/what-makes-us-smart
(What Makes Us Smart?)

\[[Serendipity][Serendipity]\]
Wendy Ross, Samantha Copeland, Stuart Firestein (2024).
Serendipity in Scientific Research. (Journal of Trial and Error)

[Serendipity]: https://journal.trialanderror.org/pub/serendipity-in-scientific/release/2
(Serendipity in Scientific Research)

\[[FailFast][FailFast]\]
Alessandro Narduzzo, Valentina Forrer (2024).
Nurturing innovation through intelligent failure: The art of failing on purpose.

[FailFast]: https://www.sciencedirect.com/science/article/pii/S0166497224000014
(Nurturing innovation through intelligent failure: The art of failing on purpose)

\[[TransferLearning][TransferLearning]\]
Stevo Bozinovski (1976).
Reminder of the First Paper on Transfer Learning in Neural Networks.

[TransferLearning]: https://www.informatica.si/index.php/informatica/article/view/2828
(Reminder of the First Paper on Transfer Learning in Neural Networks)

\[[IMO][IMO]\]
Thang Luong, Edward Lockhart (2025).
Advanced version of Gemini with Deep Think officially achieves gold-medal standard at the
International Mathematical Olympiad.

[IMO]: https://deepmind.google/blog/advanced-version-of-gemini-with-deep-think-officially-achieves-gold-medal-standard-at-the-international-mathematical-olympiad/
(Advanced version of Gemini with Deep Think officially achieves gold-medal standard at the
International Mathematical Olympiad)

\[[NaturalSelection][NaturalSelection]\]
Dan Hendrycks (2023).
Natural Selection Favors AIs over Humans.

[NaturalSelection]: https://arxiv.org/abs/2303.16200
(Natural Selection Favors AIs over Humans)

\[[SelfDomestication][SelfDomestication]\]
Brian Hare, Vanessa Woods (2021).
Survival of the Friendliest. Understanding Our Origins and Rediscovering Our Common
Humanity.

[SelfDomestication]: https://www.penguinrandomhouse.com/books/550437/survival-of-the-friendliest-by-brian-hare-and-vanessa-woods/
(Survival of the Friendliest. Understanding Our Origins and Rediscovering Our Common
Humanity)

\[[GoodnessParadox][GoodnessParadox]\]
Richard Wrangham (2019).
The Goodness Paradox: The Strange Relationship Between Virtue and Violence in Human
Evolution.

[GoodnessParadox]: https://en.wikipedia.org/wiki/The_Goodness_Paradox
(The Goodness Paradox: The Strange Relationship Between Virtue and Violence in Human
Evolution)
