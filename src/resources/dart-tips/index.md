---
reference: "https://www.dartlang.org/dart-tips/"

layout: page
title: "Dart Tips: Short Video Tutorials about Dart"
description: "Super short video intros to Dart language and library features."
---

{% injectdata tips resources/dart-tips/episodes.yaml %}

# Dart Tips: Short Video Tutorials

Sometimes, you only have 5 minutes. Watch super short introductions to
Dart language and library topics.

{% for episode in page.tips.episodes %}
{% capture link %}dart-tips-ep-{{episode.num}}.html{% endcapture %}
<a href="{{ link }}">
  <img style="margin-top:25px; box-shadow: 5px 5px 10px #CCC;" src="{{episode.thumbnail}}">
</a>
<h3><a href="{{ link }}">Ep. {{ episode.num }}: {{ episode.subtitle }}</a></h3>
<p>{{ episode.description }}</p>
<p>{{ episode.pubdate }}</p>
{% endfor %}

<a href="http://marakana.com"><img src="images/marakana-logo.png" alt="Marakana Logo"></a>
Our thanks go out to [Marakana](http://www.marakana.com) for producing this
video series.
