# CiTO annotation with the BMC LaTeX template

Author: Egon Willighagen, https://orcid.org/0000-0001-7542-0286 <br />
License: CC-BY 4.0 International

Users of the [BMC LaTeX template](http://media.biomedcentral.com/content/production/bmc_article-tex.zip) (see also
[this page](https://jcheminf.biomedcentral.com/submission-guidelines/preparing-your-manuscript)) only have to
make a small edit in their `.bib` file. Following the template, you can add a `note` field to the BiBTeX file
and wrap the `[cito:citesAsDataSource] [cito:confirms]` (:

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

