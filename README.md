About r-eikosograms
===================

Home: https://github.com/rwoldford/eikosograms

Package license: GPL-3.0-only

Feedstock license: [BSD-3-Clause](https://github.com/conda-forge/r-eikosograms-feedstock/blob/main/LICENSE.txt)

Summary: An eikosogram (ancient Greek for probability picture) divides the unit square into rectangular regions whose areas, sides, and widths, represent various probabilities associated with the values of one or more categorical variates. Rectangle areas are joint probabilities, widths are always marginal (though possibly joint margins, i.e. marginal joint distributions of two or more variates), and heights of rectangles are always conditional probabilities. Eikosograms embed the rules of probability and are useful for introducing elementary probability theory, including axioms, marginal, conditional, and joint probabilities, and their relationships (including Bayes theorem as a completely trivial consequence). They are markedly superior to Venn diagrams for this purpose, especially in distinguishing probabilistic independence, mutually exclusive events, coincident events, and associations. They also are useful for identifying and understanding conditional independence structure. As data analysis tools, eikosograms display categorical data in a manner similar to Mosaic plots, especially when only two variates are involved (the only case in which they are essentially identical, though eikosograms purposely disallow spacing between rectangles). Unlike Mosaic plots, eikosograms do not alternate axes as each new categorical variate (beyond two) is introduced. Instead, only one categorical variate, designated the "response", presents on the vertical axis and all others, designated the "conditioning" variates, appear on the horizontal. In this way, conditional probability appears only as height and marginal probabilities as widths. The eikosogram is therefore much better suited to a response model analysis (e.g. logistic model) than is a Mosaic plot. Mosaic plots are better suited to log-linear style modelling as in discrete multivariate analysis. Of course, eikosograms are also suited to discrete multivariate analysis with each variate in turn appearing as the response. This makes it better suited than Mosaic plots to discrete graphical models based on conditional independence graphs (i.e. "Bayesian Networks" or "BayesNets"). The eikosogram and its superiority to Venn diagrams in teaching probability is described in W.H. Cherry and R.W. Oldford (2003) <https://math.uwaterloo.ca/~rwoldfor/papers/eikosograms/paper.pdf>, its value in exploring conditional independence structure and relation to graphical and log-linear models is described in R.W. Oldford (2003) <https://math.uwaterloo.ca/~rwoldfor/papers/eikosograms/independence/paper.pdf>, and a number of problems, puzzles, and paradoxes that are easily explained with eikosograms are given in R.W. Oldford (2003) <https://math.uwaterloo.ca/~rwoldfor/papers/eikosograms/examples/paper.pdf>.

Current build status
====================


<table><tr><td>All platforms:</td>
    <td>
      <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=17183&branchName=main">
        <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-eikosograms-feedstock?branchName=main">
      </a>
    </td>
  </tr>
</table>

Current release info
====================

| Name | Downloads | Version | Platforms |
| --- | --- | --- | --- |
| [![Conda Recipe](https://img.shields.io/badge/recipe-r--eikosograms-green.svg)](https://anaconda.org/conda-forge/r-eikosograms) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/r-eikosograms.svg)](https://anaconda.org/conda-forge/r-eikosograms) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/r-eikosograms.svg)](https://anaconda.org/conda-forge/r-eikosograms) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/r-eikosograms.svg)](https://anaconda.org/conda-forge/r-eikosograms) |

Installing r-eikosograms
========================

Installing `r-eikosograms` from the `conda-forge` channel can be achieved by adding `conda-forge` to your channels with:

```
conda config --add channels conda-forge
conda config --set channel_priority strict
```

Once the `conda-forge` channel has been enabled, `r-eikosograms` can be installed with `conda`:

```
conda install r-eikosograms
```

or with `mamba`:

```
mamba install r-eikosograms
```

It is possible to list all of the versions of `r-eikosograms` available on your platform with `conda`:

```
conda search r-eikosograms --channel conda-forge
```

or with `mamba`:

```
mamba search r-eikosograms --channel conda-forge
```

Alternatively, `mamba repoquery` may provide more information:

```
# Search all versions available on your platform:
mamba repoquery search r-eikosograms --channel conda-forge

# List packages depending on `r-eikosograms`:
mamba repoquery whoneeds r-eikosograms --channel conda-forge

# List dependencies of `r-eikosograms`:
mamba repoquery depends r-eikosograms --channel conda-forge
```


About conda-forge
=================

[![Powered by
NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://numfocus.org)

conda-forge is a community-led conda channel of installable packages.
In order to provide high-quality builds, the process has been automated into the
conda-forge GitHub organization. The conda-forge organization contains one repository
for each of the installable packages. Such a repository is known as a *feedstock*.

A feedstock is made up of a conda recipe (the instructions on what and how to build
the package) and the necessary configurations for automatic building using freely
available continuous integration services. Thanks to the awesome service provided by
[Azure](https://azure.microsoft.com/en-us/services/devops/), [GitHub](https://github.com/),
[CircleCI](https://circleci.com/), [AppVeyor](https://www.appveyor.com/),
[Drone](https://cloud.drone.io/welcome), and [TravisCI](https://travis-ci.com/)
it is possible to build and upload installable packages to the
[conda-forge](https://anaconda.org/conda-forge) [Anaconda-Cloud](https://anaconda.org/)
channel for Linux, Windows and OSX respectively.

To manage the continuous integration and simplify feedstock maintenance
[conda-smithy](https://github.com/conda-forge/conda-smithy) has been developed.
Using the ``conda-forge.yml`` within this repository, it is possible to re-render all of
this feedstock's supporting files (e.g. the CI configuration files) with ``conda smithy rerender``.

For more information please check the [conda-forge documentation](https://conda-forge.org/docs/).

Terminology
===========

**feedstock** - the conda recipe (raw material), supporting scripts and CI configuration.

**conda-smithy** - the tool which helps orchestrate the feedstock.
                   Its primary use is in the construction of the CI ``.yml`` files
                   and simplify the management of *many* feedstocks.

**conda-forge** - the place where the feedstock and smithy live and work to
                  produce the finished article (built conda distributions)


Updating r-eikosograms-feedstock
================================

If you would like to improve the r-eikosograms recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`conda-forge` channel, whereupon the built conda packages will be available for
everybody to install and use from the `conda-forge` channel.
Note that all branches in the conda-forge/r-eikosograms-feedstock are
immediately built and any created packages are uploaded, so PRs should be based
on branches in forks and branches in the main repository should only be used to
build distinct package versions.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string)
   back to 0.

Feedstock Maintainers
=====================

* [@conda-forge/r](https://github.com/conda-forge/r/)
* [@mfansler](https://github.com/mfansler/)

