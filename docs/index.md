---
layout: default
speakers:
  - name: Robert Gentleman
    inst: 23andMe
    url: https://blog.23andme.com/23andme-research/a-computational-biologist-and-a-gentleman/
    blurb: "Robert Gentleman is currently vice president of computational biology at 23andMe. Prior to that, he was a senior director of Bioinformatics and computational biology in Genentech. He is recognized, along with Ross Ihaka, as one of the originators of the R programming language. He has also co-founded the Bioconductor project, which aims to promote the development of open-source tools for bioinformatics and computational biology."
---

{% include header.md %}

BiocAsia2020 highlights current developments within and beyond
the [Bioconductor](https://www.bioconductor.org) project. 

## Key dates

- Oct 17-18: BiocAsia2020 Meeting, Beijing

## Confirmed Speakers

{% for s in page.speakers %}
{% assign imgpath = "images/speakers/" | append: s.name | remove: ' ' | append: '.jpg' %}
<img src="{{ imgpath }}" style="float:right; width:150px; height:150px; object-fit: cover">
### [{{ s.name }}]({{ s.url }}), {{ s.inst }}

> {{ s.blurb }}

{% endfor %}

More information: [qian.liu@roswellpark.org][contact]

[contact]: mailto:qian.liu@roswellpark.org?subject=BiocAsia2020%20question

<a href="https://twitter.com/intent/tweet?button_hashtag=biocAsia2020&ref_src=twsrc%5Etfw"
    class="twitter-hashtag-button"
    data-show-count="false">Tweet #biocAsia2020</a>
