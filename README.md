# Planar equivalent layers for potential fields
## Part 1. Theoretical insights
## Part 2. Geophysical implications and applications

by Vanderlei C. Oliveira Jr<sup>1</sup>, 
Christian Gerhards<sup>2</sup>, 
Valéria C. F. Barbosa<sup>1</sup>, 
André L. A. Reis<sup>1</sup>, 
Edson F. Luza<sup>1</sup> and 
Xinpeng Huang<sup>2, 3</sup>


<sup>1</sup> Coordenação de Geofı́sica, Observatório Nacional, General José Cristino st., Rio de Janeiro, Brazil

<sup>2</sup> Institute of Geophysics and Geoinformatics, TU Bergakademie Freiberg, Gustav-Zeuner-Str., Freiberg, Germany

<sup>3</sup> School of Geosciences and Info-Physics, Central South University, South Lushan Road, Changsha Hunan, P. R. China

![](manuscript/part1/Figure1_1.png)

*2D schematic representation of sources located in subsurface and the geometrical aspects of our work.*


## Abstract -- Part 1

A comprehensive theoretical framework is developed for potential-field transformations 
based on planar equivalent layers, a technique empirically used in applied geophysics since 
the 1960s. The formulation replaces the widely accepted equivalent-layer principle -- primarily 
founded on empirical generalizations -- with a rigorous theoretical foundation. The planar 
equivalent-layer theorem establishes the existence of continuous planar layers capable of 
reproducing potential-field data exactly when they reside strictly in the source-free region above 
the sources, or within a predefined error level when they intersect the true sources
Closed-form expressions for planar equivalent layers are derived 
by modifying the classical solutions of Dirichlet's and Neumann's problems, revealing that 
these layers possess tangible physical meaning related to boundary-value problems in potential 
theory. The theoretical framework also demonstrates the mathematical equivalence between 
potential-field transformations computed via the equivalent-layer technique and those obtained 
through Fourier-domain approaches. Distinct classes of equivalent layers are formally defined, 
together with their relationships to the observed data, true sources, and potential-field 
transformations. The resulting formulation provides a rigorous explanation for the 
long-standing success of the equivalent-layer technique in potential-field analysis.

## Abstract -- Part 2

The equivalent-layer technique has been widely applied in geophysics since the 1960s 
for potential-field transformations as well as for processing and interpreting 
gravity and magnetic data. Despite its success, the method has traditionally relied 
on empirical assumptions, with limited attention to its theoretical foundation. In a 
companion paper, we have established a rigorous theoretical framework for planar equivalent layers. 
Here, we examine the implications of these theoretical results for the empirical 
approaches commonly used in the geophysical literature. Through 
numerical experiments, we demonstrate the numerical consistency and close agreement between the 
closed-form expressions for planar equivalent layers and the discrete layers obtained 
by linear inversion of potential-field data. Our results confirm that multiple planar equivalent 
layers can be employed to achieve the same potential-field transformations.


## Numerical simulations

All source code used to generate the results and figures in the paper are in the `code` folder.
The calculations and figure generation are all run inside [Jupyter notebooks](http://jupyter.org/).


## Getting the manuscript and all numerical simulations

You can download a copy of all the files in this repository by cloning the repository:

    git clone https://github.com/birocoles/planar-eqlayer-theory.git

or [download a zip archive](https://github.com/birocoles/planar-eqlayer-theory/XXXXXX/main.zip).

A copy of the repository is also archived at *insert DOI here*


## Dependencies

You'll need a working Python environment to run the code.
The recommended way to set up your environment is through the
[Anaconda Python distribution](https://www.anaconda.com/download/) which
provides the `conda` package manager.
Anaconda can be installed in your user directory and does not interfere with
the system Python installation.
The required dependencies are specified in the file `environment.yml`.

We use `conda` virtual environments to manage the project dependencies in
isolation.
Thus, you can install our dependencies without causing conflicts with your
setup (even with different Python versions).

Run the following command in the repository folder (where `environment.yml`
is located) to create a separate environment and install all required
dependencies in it:

    conda env create


## Reproducing the results

Before running any code you must activate the conda environment:

    source activate ENVIRONMENT_NAME

or, if you're on Windows:

    activate ENVIRONMENT_NAME

This will enable the environment for your current terminal session.
Any subsequent commands will use software that is installed in the environment.

To build and test the software, produce all results and figures, and compile
the manuscript PDF, run this in the top level of the repository:

    make all

If all goes well, the manuscript PDF will be placed in `manuscript/output`.

You can also run individual steps in the process using the `Makefile`s from the
`code` and `manuscript` folders. See the respective `README.md` files for
instructions.

Another way of exploring the code results is to execute the Jupyter notebooks
individually.
To do this, you must first start the notebook server by going into the
repository top level and running:

    jupyter notebook

This will start the server and open your default web browser to the Jupyter
interface. In the page, go into the `code/notebooks` folder and select the
notebook that you wish to view/run.

The notebook is divided into cells (some have text while other have code).
Each cell can be executed using `Shift + Enter`.
Executing text cells does nothing and executing code cells runs the code
and produces it's output.
To execute the whole notebook, run all cells in order.


## License

All source code is made available under a BSD 3-clause license. You can freely
use and modify the code, without warranty, so long as you provide attribution
to the authors. See `LICENSE.md` for the full license text.

The manuscript text is not open source. The authors reserve the rights to the
article content, which is currently submitted for publication in the
Journal of Geophysical Research: Solid Earth.
