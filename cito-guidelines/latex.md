# CiTO annotation with the BMC LaTeX template

Author: Egon Willighagen, https://orcid.org/0000-0001-7542-0286 <br />
License: CC-BY 4.0 International

Users of the [BMC LaTeX template](http://media.biomedcentral.com/content/production/bmc_article-tex.zip) (see also
[this page](https://jcheminf.biomedcentral.com/submission-guidelines/preparing-your-manuscript)) only have to
make a small edit in their `.bib` file. Following the template, you can add a `note` field to the BiBTeX file
and wrap the `[cito:citesAsDataSource]` in an `\textbf{}`:

```bibtex
@article{koon,
  author  = {Koonin, E V and Altschul, S F and P Bork}, 
  title   = {BRCA1 protein products: functional motifs}, 
  journal = {Nat Genet}, 
  year    = {1996},
  volume  = {13}, 
  pages   = {266-267},
  note      = {\textbf{[cito:citesAsDataSource]}}
}
```

or for two CiTO annotations, `[cito:citesAsDataSource] [cito:confirms]`, like this:

```bibtex
@book{marg,
  author    = {L Margulis}, 
  title     = {Origin of Eukaryotic Cells},
  publisher = {Yale University Press}, 
  year      = {1970},
  address   = {New Haven},
  note      = {\textbf{[cito:citesAsDataSource] [cito:confirms]}}
}
```

