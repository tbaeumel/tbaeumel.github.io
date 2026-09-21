---
permalink: /
title: "About me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a fourth-year PhD student in the Multilinguality and Language Technology lab at the German Research Center for Artificial Intelligence (DFKI), supervised by Josef van Genabith and Simon Ostermann.

In my PhD thesis, I study what happens inside large language models when they solve challenging tasks. LLMs often look impressive, but their performance frequently rests on simple heuristics that make them brittle. Using interpretability methods, I trace the mechanisms behind these shortcuts to understand why they form and how to overcome them.

Beyond my thesis, I am broadly interested in how language models work on the inside:

- **Mechanistic interpretability:** reverse-engineering the internal mechanisms behind model behavior, and using these insights to improve models
- **Tokenization:** how the choice of tokens shapes what a model has to learn and how it represents it
- **Reasoning mechanisms:** how LLMs solve arithmetic and other reasoning tasks internally

<!-- Old intro:
I am a 4th year PhD student and researcher in the Multilinguality and Language Technology lab at the German Research Center for Artificial Intelligence, working under the supervision of Josef van Genabith and Simon Ostermann. 
My research is in the field of interpretable artificial intelligence, where I work on understanding the inner workings of large-scale pre-trained language models, as well as understanding and overcoming their limitations.
My background is in computational linguistics, computer science and cognitive science.
-->

News
------

<ul class="news">
{% assign news_items = site.data.news | sort: "date" | reverse %}
{% for item in news_items limit: 6 %}
  <li><strong>{{ item.date | date: "%b %Y" }}</strong> &ndash; {{ item.text | markdownify | remove: '<p>' | remove: '</p>' | strip }}</li>
{% endfor %}
</ul>

Thesis topics 
------

I am always looking for talented Master students of Language Science and Technology or Computer Science, who want to work on a thesis in the area of interpretable, robust, or trustworty NLP. 

If you are interested, feel free to reach out with your own research question related to my research interests above.

When contacting me, please include:
- Your CV
- Your Transcript of Records
- A short research question pitch (possibly accompanied with relevant literature that your idea builds on)

<!-- Old research interests:
Current Research Interests: 
- **(Actionable) Mechanistic Interpretability**: Understanding how LLMs work and using interpretability insights to improve them
- **Model Editing and Machine Unlearning:** Methods for editing or forgetting knowledge in LLMs
- **Reasoning in LLMs:** Exploring arithmetic, chain-of-thought (CoT), or other reasoning processes
-->
