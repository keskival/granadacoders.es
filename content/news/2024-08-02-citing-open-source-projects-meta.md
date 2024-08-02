---
title: "Meta FAIR refuses to cite my open source project to maintain a claim of novelty"
date: 2024-08-02
author: Tero Keski-Valkama
draft: false
---

I have been working in AI for decades ([1](https://www.linkedin.com/in/terokeskivalkama/) [2](https://scholar.google.com/citations?user=l7qMBpkAAAAJ)). In the end of 2023 I started talking about bootstrapping recursive self-improvement
of LLM chatbots using two key ideas:
1. Open-ended, non-imitative objectives, because imitative objectives are capped at the human level.
2. Using automatic evaluation or ranking of performances by LLMs, but crucially evaluating the act of evaluation as well so that evaluation fidelity also improves and exceeds the human level.

At some point I decided that large corporate labs aren't moving on this fast enough, so I started an open source project: [Recursive Self-improvement Suite](https://github.com/keskival/recursive-self-improvement-suite).

The project is just a proof-of-concept, describing the hypothesis and running the tasks, their evaluations and evaluations of the evaluations
on OpenAI ChatGPT-3.5. It produces ranked data which can be used for reinforcement learning, DPO or even supervised continual training
to improve the model performance on these kinds of open ended tasks.

In July 2023 Meta FAIR published a pre-print on Arxiv titled: [Meta-Rewarding Language Models: Self-Improving Alignment with LLM-as-a-Meta-Judge](https://arxiv.org/abs/2407.19594).

This pre-print describes the exact idea of evaluating the evaluations which I had described before, with a meta-judge.

Here is what I wrote in the project:
![Screenshot of the project README, parts highlighted describing evaluating the evaluations](/imgs/meta-refuses-to-cite-my-project.png)

I had also implemented this already ages ago [here](https://github.com/keskival/recursive-self-improvement-suite/blob/bb327635885a3c3f1a4c1fca5e5f649dd6e53295/python/recursive_self_improvement_suite/coding.py#L338-L384).

This is what their article says, describing this as a "novel method", proposed by them:
![Screenshot of the paper, parts highlighted describing evaluating the evaluations](/imgs/meta-refuses-to-cite-their-paper.png)

These are describing the same thing, although their paper assigns scores out of 5, while my project ranks. Ranking is of course a superior option because it's open ended by nature, and won't get stuck at the top score.

So, this is an understandable omission. People don't often Google or search existing art on GitHub, although it could be argued GitHub projects are more peer reviewed (by stars) than Arxiv preprints are. I do expect to be cited though, that's why the project has "Citing" section in the README.md, giving a convenient BibTex snippet for it.

I sent them an email to the email address who submitted the paper to Arxiv.

They responded very fast: "Thanks for the link.. ! Respectfully, not sure that's quite enough to warrant a citation -- but definitely good to brainstorm and try stuff!":

![Screenshot of the email](/imgs/meta-refuses-to-cite-their-response.png)

It is natural that they don't want to cite existing art because it invalidates their claim of novelty. Furthermore, I would say my method
is actually an evolution over theirs, because it ranks instead of scores, and also it ranks problem creation task as well.

It is however a severe breach of scientific ethics. They cannot claim proposing a novelty when someone else has proposed it before.

This is erasing independent researchers from the history of science and claiming credit for their inventions.

I am obviously not happy about this. I am myself trying to complete my Dr.Sc.(Tech.) degree with peer reviewed publications and it undermines
my efforts if credit that properly belongs to the first inventor of a method is stolen.

Here are some posts where more discussion about this is happening. Feel free to share to science journalists or influencers, or other relevant parties!

- [LinkedIn post](https://www.linkedin.com/posts/terokeskivalkama_meta-fair-fails-to-cite-my-pre-existing-publication-activity-7224732917132894209-WYKA)
- [Mastodon post](https://rukii.net/@tero/112886575304660317)
- [Facebook post](https://www.facebook.com/KohrAh/posts/pfbid02mc3PNxESy55M8uj6i9iD4uw69YjaoTWUy5J9RX4XfxAZ6Nnj8Prx2nE85WJKJmdql)
