---
layout: default
---

{% include header.md %}

## Workshops

Join the *Bioconductor*
[\#biocasia2020](https://community-bioc.slack.com/archives/CSF3EKY0Y) channel for up-to-date information.

### Chinese (中文)

| Workshop                                                                                                                 | Source                                                                                             | Docker                                                                                                                  |
| :----------------------------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------- |
| [使用limma、Glimma和edgeR，RNA-seq数据分析易如反掌](https://xueyidong.github.io/RNAseq123CN/)                             | [![GH](images/GitHub-Mark-32px.png)](https://github.com/XueyiDong/RNAseq123CN)                      | [![Docker](images/docker_icon.png)](https://hub.docker.com/r/xueyidong/rnaseq123cn)                      |
| [Analysis and visualization of microbiome datasets using MicrobiotaProcess](https://yulab-smu.top/MicrobiotaProcessWorkshop/)                             | [![GH](images/GitHub-Mark-32px.png)](https://github.com/YuLab-SMU/MicrobiotaProcessWorkshop)                      | [![Docker](images/docker_icon.png)](https://hub.docker.com/r/xushuangbin/microbiotaprocess_workshop)                      |
| [An introduction to single-cell RNA-sequencing analysis in Bioconductor](https://you-k.github.io/scRNA-seq-workshop/)                             | [![GH](images/GitHub-Mark-32px.png)](https://github.com/YOU-k/scRNA-seq-workshop)                      | [![Docker](images/docker_icon.png)](https://hub.docker.com/u/chloeyou/scRNA-seq-workshop)                      |

<sup></sup>

### English

| Workshop                                                                                                                 | Source                                                                                             | Docker                                                                                                                  |
| :----------------------------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------- |
| [trackViewer: Lollipop/Dandelion plots for methylation status and mutation data](https://jianhong.github.io/trackViewerBiocAsia2020Workshop/)                             | [![GH](images/GitHub-Mark-32px.png)](https://github.com/jianhong/trackViewerBiocAsia2020Workshop)                      | [![Docker](images/docker_icon.png)](https://hub.docker.com/r/jianhong/trackviewerbiocasia2020workshop)                      |
| [Building a Bioconductor package](https://saskiafreytag.github.io/making_bioconductor_pkg)                             | [![GH](images/GitHub-Mark-32px.png)](https://github.com/SaskiaFreytag/making_bioconductor_pkg)                      | [![Docker](images/docker_icon.png)](https://hub.docker.com/r/saskiafreytag/making_bioconductor_pkg)                      |
| [Bioconductor toolchain for usage and development of reproducible bioinformatics pipelines in CWL](https://liubuntu.github.io/Bioc2020RCWL/)                             | [![GH](images/GitHub-Mark-32px.png)](https://github.com/Liubuntu/Bioc2020RCWL)                      | [![Docker](images/docker_icon.png)](https://hub.docker.com/repository/docker/liubuntu/bioc2020rcwl)                      |
| [How to perform analysis of RNA sequencing data following the tidy data paradigm](https://stemangiola.github.io/biocasia2020_tidytranscriptomics/)                             | [![GH](images/GitHub-Mark-32px.png)](https://github.com/stemangiola/biocasia2020_tidytranscriptomics)                      | [![Docker](images/docker_icon.png)](https://hub.docker.com/r/stemangiola/biocasia2020_tidytranscriptomics)                      |
| [Hands-on experience to CiteFuse that consists of a suite of tools for the integration and the downstream analysis of CITE-seq data](https://sydneybiox.github.io/BiocAsia2020CiteFuse)                             | [![GH](images/GitHub-Mark-32px.png)](https://github.com/SydneyBioX/BiocAsia2020CiteFuse)                      | [![Docker](images/docker_icon.png)](https://hub.docker.com/r/yingxinlin/biocasia2020citefuse)                      |

<sup></sup>

Workshops with preinstalled dependencies can be run locally using
Docker.

  - `docker pull <userid/workshop:latest>` will pull the latest image
    for a given `<workshop>`.
  - `docker run -e PASSWORD=<yourpassword> -p 8787:8787 -d --rm
    <userid/workshop>` will publish a container’s port 8787 to the host
    (`-p`), run in the detached mode (`-d`), and cleanly remove the
    container when it is stopped (`--rm`).
  - Open <http://localhost:8787> and login with username `rstudio` and
    password `<yourpassword>`.
  - Run `browseVignettes(package = "<workshop>")`. Click on one of the
    links, “HTML”, “source”, “R code”.
      - In case of “`The requested page was not found`” error, add
        `help/` to the URL right after the hostname. This is a [known
        bug](https://github.com/rocker-org/rocker-versioned/issues/178).

Advanced: Use `-v $(pwd):/home/rstudio` argument to map your local
directory to the container. Use `-e DISABLE_AUTH=true`, if you want
passwordless login to RStudio. On Windows, you may need to provide your
localhost IP address like `http://191.163.92.108:8787/` - find it using
`docker-machine ip default` in Docker’s terminal.

Example:

    docker pull waldronlab/publicdataresources:latest
    docker run -e PASSWORD=bioconductor -p 8787:8787 -d --rm waldronlab/publicdataresources
    # Open http://localhost:8787 and login using rstudio/bioconductor credentials
    # Run browseVignettes(package = "PublicDataResources")
    # Open http://localhost:8787/help/library/PublicDataResources/doc/PublicDataResources.html
    docker ps -a # List all running containers
    docker stop <CONTAINER ID> # or, <NAMES> - Stop a container

Workshop packages were created using the
[BuildABiocWorkshop2020](https://github.com/seandavi/BuildABiocWorkshop2020)
template.

*NOTE*. All workshops should include a valid `DESCRIPTION` file with the
following fields:

  - `URL:` - the GitHub pages URL
    (`https://username.github.io/repository`)
  - `DockerImage:` - the Docker repository slug in lowercase with
    (optional) tag (`username/repository:tag`)
