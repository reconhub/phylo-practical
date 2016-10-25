
# Introduction to phylogenetics using R

This practical provides an overview of different phylogenetic reconstruction methods in R, using influenza virus sequences. 

**Click on the tree to access the pdf:**

<a href="https://raw.githubusercontent.com/reconhub/phylo-practical/master/phylo-practical.pdf"><img src="ygg.jpg" alt="link to pdf"  width="300px"></a>




<br>

# Content of the repository

This repository contains the following files:

- [`phylo-practical.Rnw`](https://raw.githubusercontent.com/reconhub/phylo-practical/master/phylo-practical.Rnw): the *knitr* document of the practical
- [`phylo-practical.pdf`](https://raw.githubusercontent.com/reconhub/phylo-practical/master/phylo-practical.pdf): the pdf version of the practical; to recompile it freshly, use: `knitr::knit2pdf("phylo-practical.Rnw")`
- `data/`: a folder containing two datasets:
  - [`usflu.annot.csv`](https://raw.githubusercontent.com/reconhub/phylo-practical/master/data/usflu.annot.csv): annotations of the sequences
  - [`usflu.fasta`](https://raw.githubusercontent.com/reconhub/phylo-practical/master/data/usflu.fasta): a *fasta* file containing aligned sequences
- `figs/`: figures produced by *knitr* as well as images used to generate the pdf



<br>

# Compiling this document yourself

To compile this document, you first need to download a handful of files:

```r
## file URLs
base.url <- "https://raw.githubusercontent.com/reconhub/phylo-practical/master/"
files.to.get <- c("phylo-practical.Rnw", "biblioTJ.bib", "Rlogo.pdf", "ygg.jpg")
urls <- paste0(base.url, files.to.get)

## set working directory - change 'dest.dir' as you want
dest.dir <- "phylo-practical"
if (!dir.exists(dest.dir)) dir.create(dest.dir)
setwd(dest.dir)
dir.create("figs")

## download files
for (i in seq_along(urls)) {
  download.file(urls[[i]], files.to.get[i], method = "curl")
}
```

And then compile the document using:

```r
knitr::knit2pdf("phylo-practical.Rnw")
```



<br>

# Feedback & contributions

Please send feedback using the [issues](http://github.com/reconhub/phylo-practical/issues) system. Contributions are welcome as pull requests.



<br>

# Credits

Author: [Thibaut Jombart](https://sites.google.com/site/thibautjombart/)

Licence: this work is released under [Creative Common Attribution 4.0](http://creativecommons.org/licenses/by/4.0/).

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons Licence" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a>



