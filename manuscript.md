---
author-meta:
- Taylor Ferebee
- Jane Roe
bibliography:
- content/manual-references.json
date-meta: '2020-08-28'
header-includes: '<!--

  Manubot generated metadata rendered from header-includes-template.html.

  Suggest improvements at https://github.com/manubot/manubot/blob/master/manubot/process/header-includes-template.html

  -->

  <meta name="dc.format" content="text/html" />

  <meta name="dc.title" content="Prediction-based evaluation of community detection methods for maize gene expression data" />

  <meta name="citation_title" content="Prediction-based evaluation of community detection methods for maize gene expression data" />

  <meta property="og:title" content="Prediction-based evaluation of community detection methods for maize gene expression data" />

  <meta property="twitter:title" content="Prediction-based evaluation of community detection methods for maize gene expression data" />

  <meta name="dc.date" content="2020-08-28" />

  <meta name="citation_publication_date" content="2020-08-28" />

  <meta name="dc.language" content="en-US" />

  <meta name="citation_language" content="en-US" />

  <meta name="dc.relation.ispartof" content="Manubot" />

  <meta name="dc.publisher" content="Manubot" />

  <meta name="citation_journal_title" content="Manubot" />

  <meta name="citation_technical_report_institution" content="Manubot" />

  <meta name="citation_author" content="Taylor Ferebee" />

  <meta name="citation_author_institution" content="Department of Computational Biology, Cornell University" />

  <meta name="citation_author_orcid" content="XXXX-XXXX-XXXX-XXXX" />

  <meta name="twitter:creator" content="@Ferebee2PhD" />

  <meta name="citation_author" content="Jane Roe" />

  <meta name="citation_author_institution" content="Department of Something, University of Whatever" />

  <meta name="citation_author_institution" content="Department of Whatever, University of Something" />

  <meta name="citation_author_orcid" content="XXXX-XXXX-XXXX-XXXX" />

  <link rel="canonical" href="https://thferebee.github.io/PhenoEval-Coexpress-manubot/" />

  <meta property="og:url" content="https://thferebee.github.io/PhenoEval-Coexpress-manubot/" />

  <meta property="twitter:url" content="https://thferebee.github.io/PhenoEval-Coexpress-manubot/" />

  <meta name="citation_fulltext_html_url" content="https://thferebee.github.io/PhenoEval-Coexpress-manubot/" />

  <meta name="citation_pdf_url" content="https://thferebee.github.io/PhenoEval-Coexpress-manubot/manuscript.pdf" />

  <link rel="alternate" type="application/pdf" href="https://thferebee.github.io/PhenoEval-Coexpress-manubot/manuscript.pdf" />

  <link rel="alternate" type="text/html" href="https://thferebee.github.io/PhenoEval-Coexpress-manubot/v/095ac3d343c7d0ed6d428496cc9de31d14c5e5c6/" />

  <meta name="manubot_html_url_versioned" content="https://thferebee.github.io/PhenoEval-Coexpress-manubot/v/095ac3d343c7d0ed6d428496cc9de31d14c5e5c6/" />

  <meta name="manubot_pdf_url_versioned" content="https://thferebee.github.io/PhenoEval-Coexpress-manubot/v/095ac3d343c7d0ed6d428496cc9de31d14c5e5c6/manuscript.pdf" />

  <meta property="og:type" content="article" />

  <meta property="twitter:card" content="summary_large_image" />

  <link rel="icon" type="image/png" sizes="192x192" href="https://manubot.org/favicon-192x192.png" />

  <link rel="mask-icon" href="https://manubot.org/safari-pinned-tab.svg" color="#ad1457" />

  <meta name="theme-color" content="#ad1457" />

  <!-- end Manubot generated metadata -->'
keywords:
- coexpression
- community-detection
- gene-expression
lang: en-US
manubot-clear-requests-cache: false
manubot-output-bibliography: output/references.json
manubot-output-citekeys: output/citations.tsv
manubot-requests-cache-path: ci/cache/requests-cache
title: Prediction-based evaluation of community detection methods for maize gene expression data
...






<small><em>
This manuscript
([permalink](https://thferebee.github.io/PhenoEval-Coexpress-manubot/v/095ac3d343c7d0ed6d428496cc9de31d14c5e5c6/))
was automatically generated
from [thferebee/PhenoEval-Coexpress-manubot@095ac3d](https://github.com/thferebee/PhenoEval-Coexpress-manubot/tree/095ac3d343c7d0ed6d428496cc9de31d14c5e5c6)
on August 28, 2020.
</em></small>

## Authors



+ **Taylor Ferebee**<br>
    ![ORCID icon](images/orcid.svg){.inline_icon}
    [XXXX-XXXX-XXXX-XXXX](https://orcid.org/XXXX-XXXX-XXXX-XXXX)
    · ![GitHub icon](images/github.svg){.inline_icon}
    [thferebee](https://github.com/thferebee)
    · ![Twitter icon](images/twitter.svg){.inline_icon}
    [Ferebee2PhD](https://twitter.com/Ferebee2PhD)<br>
  <small>
     Department of Computational Biology, Cornell University
     · Funded by Grant XXXXXXXX
  </small>

+ **Jane Roe**<br>
    ![ORCID icon](images/orcid.svg){.inline_icon}
    [XXXX-XXXX-XXXX-XXXX](https://orcid.org/XXXX-XXXX-XXXX-XXXX)
    · ![GitHub icon](images/github.svg){.inline_icon}
    [janeroe](https://github.com/janeroe)<br>
  <small>
     Department of Something, University of Whatever; Department of Whatever, University of Something
  </small>



## Abstract {.page_break_before}




## Visual Abstract


## Introduction
Since the early days of microarray experiments, much of biology has focused on inferring gene function on a global scale through the creation of gene coexpression networks. Gene co-expression networks (GCNs) are an intuitive way to understand the relationships between genes with simialar gene expresssion profiles. In these networks, nodes represent genes and thhe connection between genes (edges) provide a visual 

These relations are often found through mathematical methods such as Pearson correlation, mutual information


## Materials and Methods
### Community Detection Methods

__Hierarchical Clustering on a Topological Overlap Matrix__
One of the most common clustering methods, agglomerative heiarcarchical clustering (implemented in WGCNA R package) attempts to create a heirarchy of clusters by starting with individual clusters and building to one cluster with all data. To begin the procedure, each gene is in its own cluster and a similarity (distance) matrix is considered. If two clusters (genes) are similar (close in distance), these two genes merge. If two clusters are not close, their clusters do not merge. Once again, we consider a similarity matrix between the newly formed clusters. This repeats until all clusters have merged into a single cluster. Most often, heirarchical clustering is pressented in a dendrogram form which tracks the merges of the clusters. 

__Fast Greedy__
Fast greedy community detection uses topological features of a network and an agglomative algorithm for detecting community structure. The fast greedy algorithm utilizes a network's modularity. The modularity measures the relationship between the density of links within communities compared with the rest of the network. In other words, a particilarly modular network (as biological networks are assumed to be) have commiunityes that are very connected iwhtin the community, but only have a few edges to other communities. 


## Results


## Discussion


## References {.page_break_before}

<!-- Explicitly insert bibliography here -->
<div id="refs"></div>
