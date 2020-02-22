---
layout: default
speakers:
  - name: Robert Gentleman
    inst: 23andMe
    url: https://blog.23andme.com/23andme-research/a-computational-biologist-and-a-gentleman/
    blurb: "Robert Gentleman is currently vice president of computational biology at 23andMe. Prior to that, he was a senior director of Bioinformatics and computational biology in Genentech. He is recognized, along with Ross Ihaka, as one of the originators of the R programming language. He has also co-founded the Bioconductor project, which aims to promote the development of open-source tools for bioinformatics and computational biology."
  - name: Yi Xing
    inst: Center for Computational and Genomic Medicine, Children’s Hospital of Philadelphia
    url: https://xinglab.org/people/yi-xing/
    blurb: "Dr. Yi Xing is the Francis West Lewis Endowed Chair and Founding Director of the Center for Computational and Genomic Medicine at the Children’s Hospital of Philadelphia (CHOP), and Professor of Pathology and Laboratory Medicine at the University of Pennsylvania (Penn). Dr. Xing has an extensive publication record in bioinformatics, genomics, and RNA biology. His work has provided fundamental insights into the function, regulation, and evolution of post-transcriptional RNA processing in mammals. His current research merges the fields of computational biology, biomedical data science, RNA genomics, human genetics, precision medicine, and immuno-oncology."
  - name: Lihua Julie Zhu
    inst: University of Massachusetts Medical School
    url:  https://profiles.umassmed.edu/display/129880
    blurb: "Lihua Julie Zhu is currently a professor and the head of Bioinformatics Core in the Department of Molecular, Cell and Cancer Biology (MCCB) of University of Massachusetts Medical School (UMMS). Her group has developed a dozen Bioconductor packages with various utilities including peak annotation (ChIPpeakAnno), motif analysis and visualization (motifStack and dagLogo), ATAC-seq data evaluation (ATACseqQC), polyadenylation site identification (cleanUpdTSeq and InPAS), multi-omics data integration and visualization (trackViewer and geneNetworkBuilder), nucleolar-associated domain finder (NADfinder), and gRNA design and evaluation (CRISPRseek and GUIDEseq) for the CRISPR genome editing system."
  - name: Saskia Freytag 
    inst:  Harry Perkins Institute of Medical Research, Australia
    blurb: "Saskia Freytag is currently a post-doctoral researcher focusing on single cell omics at the Harry Perkins Institute of Medical Research. She is the developer and maintainer of several Bioconductor packages and interactive applications. For several years, she was one of the co-organizer of R-Ladies Melbourne, a diversity initiative aiming to promote gender diversity in the R community. She is also the co-host of a podcast about the R language."
  - name: Charity Law
    inst: Walter and Eliza Hall Institute of Medical Research, Australia
    blurb: "Charity Law is a statistical bioinformatician whose work focuses predominantly on gene expression analyses of high-throughput data. The impact of her work is best illustrated by the popularity of limma-voom, a method for RNA-seq gene expression analysis that she developed. She currently holds the position of senior research officer in the Epigenetics and Development Division at Walter and Eliza Hall Institute of Medical Research, Australia. In addition to differential gene expression, her research interests include differential isoform usage and transcript expression analyses, as well as exploration into methods for long-read RNA-seq and single-cell RNA-seq data."
  - name: Koki Tsuyuzaki
    inst: RIKEN BDR BiT, Japan
    blurb: "Koki Tsuyuzaki is a post-doc researcher at RIKEN BDR BiT and also a researcher at JST PRESTO. He is one of the active Bioconductor committers and has developed hundreds of R/Bioconductor packages including metaSeq, MeSH.db, MeSH.AOR.db, MeSH.PCR.db, MeSH.XXX.eg.db, MeSHDbi, LRBase.XXX.eg.db, LRBaseDbi, scTensor, and scTGIF. He will talk about the data integration approach based on tensor decomposition and the applications to single-cell omics." 
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
