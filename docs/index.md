---
layout: default
speakers:
  - name: Robert Gentleman
    inst: 23andMe
    url: https://blog.23andme.com/23andme-research/a-computational-biologist-and-a-gentleman/
    blurb: "Robert Gentleman is currently vice president of computational biology at 23andMe. Prior to that, he was a senior director of Bioinformatics and computational biology in Genentech. He is recognized, along with Ross Ihaka, as one of the originators of the R programming language. He has also co-founded the Bioconductor project, which aims to promote the development of open-source tools for bioinformatics and computational biology."
  - name: Lihua Julie Zhu
    inst: University of Massachusetts Medical School
    url: https://www.umassmed.edu/mccb/faculty-MCCB/faculty-MCCB/faculty-profile-pages/zhu-julie/
    blurb: "Dr. Lihua Julie Zhu is the head of the Bioinformatics Core in the department of Molecular, Cell and Cancer Biology, UMMC. Her work is devoted to the understanding of gene regulation and cancer biology, biomarker discovery, and development and application of gene editing technology by mining and integrating various high-throughput datasets. Her expertise is algorithm and computational biology development. Her group has developed a dozen packages with various utilities, ranging from gRNA design, machine learning application, peak calling, motif alignment, quality assessment, annotation, data integration to visualization."   
  - name: Yi Xing
    inst: Center for Computational and Genomic Medicine, Children’s Hospital of Philadelphia
    url: https://xinglab.org/people/yi-xing/
    blurb: "Dr. Yi Xing is the Francis West Lewis Endowed Chair and Founding Director of the Center for Computational and Genomic Medicine at the Children’s Hospital of Philadelphia (CHOP), and Professor of Pathology and Laboratory Medicine at the University of Pennsylvania (Penn). His current research merges the fields of computational biology, biomedical data science, RNA genomics, human genetics, precision medicine, and immuno-oncology."
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
