
# Introduction to phylogenetics using R

This practical provides an overview of different phylogenetic reconstruction methods in R, using Rusing influenza virus sequences. Useful files are:

- [`phylo-practical.Rnw`](https://raw.githubusercontent.com/reconhub/phylo-practical/master/phylo-practical.Rnw): the *knitr* document of the practical
- `phylo-practical.pdf`: the pdf version of the practical; to recompile it freshly, use: `knitr::knit2pdf("phylo-practical.Rnw")`
- `data/`: a folder containing two datasets:
  - `usflu.annot.csv`: annotations of the sequences
  - `usflu.fasta`: a *fasta* file containing aligned sequences
- `figs/`: figures produced by *knitr* as well as images used to generate the pdf



# Feedback & contributions

Please send feedback using the [issues](issues) system. Contributions are welcome as pull requests.



# Credits

Author: [Thibaut Jombart](https://sites.google.com/site/thibautjombart/)

Licence: this work is released under [Creative Common Attribution 4.0](http://creativecommons.org/licenses/by/4.0/).

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons Licence" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a>



