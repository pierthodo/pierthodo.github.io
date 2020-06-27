---
layout: home
title: Blog
---
My research interests lie at the intersection of theory and practice in Machine Learning. Considering practical problems is essential in identifying critical theme to be addressed from a more theoretical perspective. Practically, I am interested in applications of machine learning in natural science (physics, chemistry) and healthcare. More theoretically, my recent works have been focusing on data-driven sequential decision making (control theory, reinforcement learning), causality and deep learning.

I am starting a PhD at Cambridge University in the fall 2020 supervised by Prof Lawrence. Before that, I was a researcher in the MILA institute under the supervision of Prof Pineau and working towards a Master’s Degree in Computer Science at McGill University. During the summer of 2017 I was an intern at IBM Research Israel in the Machine Learning for Healthcare group under the supervision of Dr El-Hay. My first degree was in Mathematics and Computer Science at McGill University.


{% for post in site.posts %}
  <article>
    <h2>
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
    </h2>
    <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time>
    {{ post.content }}
  </article>
{% endfor %}
