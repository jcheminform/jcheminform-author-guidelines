# CiTO annotation with the BMC LaTeX template

Author: Egon Willighagen, https://orcid.org/0000-0001-7542-0286 <br />
License: CC-BY 4.0 International

Users of the [JCheminform Markdown template](https://github.com/jcheminform/markdown-jcheminf-research)
is under development and being tested as option to submit articles to the journal. The setup is similar
to that of LaTeX and you need a local processor (pandoc) to convert PDF (for preprint servers) or a Word `.docx`
document for submission to the journal.

One important different, is that this template annotates the citation at citation level, and not in the
bibliography. Therefore, the CiTO annotation must not be included as notes in the `.bib` bibliography file.
And entry has the normal form, and looks like:

```bibtex
@article{koon,
  author  = {Koonin, E V and Altschul, S F and P Bork}, 
  title   = {BRCA1 protein products: functional motifs}, 
  journal = {Nat Genet}, 
  year    = {1996},
  volume  = {13}, 
  pages   = {266-267}
}
```

In the Markdown, a citation is made by adding an `\@someBibTeXKey`. To add the CiTO intention annotation,
you would replace this with for example `\@uses_method_in:someBibTeXKey`. The template has examples.

Initial results indicate that it works too in RStudio.
