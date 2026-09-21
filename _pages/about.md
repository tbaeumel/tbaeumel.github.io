---
permalink: /
title: "About me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a 4th year PhD student and researcher in the Multilinguality and Language Technology lab at the German Research Center for Artificial Intelligence, working under the supervision of Josef van Genabith and Simon Ostermann. 
My research is in the field of interpretable artificial intelligence, where I work on understanding the inner workings of large-scale pre-trained language models, as well as understanding and overcoming their limitations.
My background is in computational linguistics, computer science and cognitive science.

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

If you are interested, feel free to reach out with your own research question related to one of the topics below.

When contacting me, please include:
- Your CV
- Your Transcript of Records
- A short research question pitch (possibly accompanied with relevant literature that your idea builds on)

Current Research Interests: 
- **(Actionable) Mechanistic Interpretability**: Understanding how LLMs work and using interpretability insights to improve them
- **Model Editing and Machine Unlearning:** Methods for editing or forgetting knowledge in LLMs
- **Reasoning in LLMs:** Exploring arithmetic, chain-of-thought (CoT), or other reasoning processes