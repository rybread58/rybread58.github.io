---
layout: default
title: Home
---

# Hello and Welcome!

Hi, this is my personal public notes/ website. I have for some time enjoyed the concept of [digital gardens](https://joelhooks.com/digital-garden/) on the internet. The concept is one in which you maitain your notes and thoughts in much the same way you might tend your garden in the backyard. Personally, I like the idea that digital gardens are less of a task, or a focus on the outcome and more on the journey that we take to get there. You write a note not always because you expect somone else to read it, but because you simply want to retain the information that you get in some fasion. That is my main goal of this website, a place to keep my thoughts and ideas and to nurture them overtime. 

## Blog vs Digital Garden

In the age of constant adds and attention grabbing headlines, I have found that blogs are starting to become the best place to relax and read. The corner of the internet that brings much less anxiety. Sometimes you read about someones thoughts, or about a new technology that the individual knows alot about. Those kinds of articles are the best. It's like having a conversation with that person at your local coffee shop. However, they have always seemed to me to be a final product kind of work. Lots of work and energy is placed in it, and then its published. Never to be edited, only to maybe be recalled in later works. To me, that seems to final. Maybe its because I am an axious person at heart, but I'd would appreciate the option to change. When you garden, nothing is really final. Sure there is often a time when things really kick off. Flowers bloom, your tomatoes grow and are plucked. But that is never the end, not really. Same goes for the notes here. They are constantly changing, unfinished, messy. I have grouped my notes more so on the stage of life they are at. Some more developed than others. All are subject to change. 



## Recently Added

{% assign all_notes = site.planted-notes | concat: site.growing-notes | concat: site.full-notes %}
{% for note in all_notes limit:5 %}
  {% unless note.path contains 'place' %}
- [{{ note.title }}]({{ note.url }})
  {% endunless %}
{% endfor %}
