# BIOMD0000000190: Model_1

## Installation

Download this repository, and install with distutils

`python setup.py install`

Or, install using pip

`pip install git+https://github.com/biomodels/BIOMD0000000190.git`

To install a specific version (in this example, from the 2014-09-16 BioModels release)

`pip install git+https://github.com/biomodels/BIOMD0000000190.git@20140916`

## Usage

Importing the model package.

`import BIOMD0000000190 as model`

Get the SBML string from the model

`print model.sbmlString`

If [python-libsbml](https://pypi.python.org/pypi/python-libsbml) bindings are
installed, the libsbml.SBMLDocument object is also accessible

`model.sbml`


# Model Notes


SBML creators: Armando Reyes-Palomares * , Carlos Rodríguez-Caso +, Raul
Montañez * , Marta Cascante $, Francisca Sánchez-Jiménez * , Miguel A. Medina
*

* ProCel Group, Department of Molecular Biology and Biochemistry, Faculty of Sciences, Campus de Teatinos, University of Malaga and CIBER de Enfermedades Raras (CIBER-ER). + Complex Systems Lab (ICREA-UPF), Barcelona Biomedical Research Park (PRBB-GRIB). $ Department of Biochemistry and Molecular Biology, Faculty of Biology, Universitat de Barcelona.

http://asp.uma.es

Metabolic modeling of polyamine metabolism in mammals.  
Rodríguez-Caso,C et al.: J Biol Chem 2006 : 281:21799-812.  
The model reproduces the dynamical behavior of the polyamine metabolism in
mammals. In this model there are some additions and corrections to the
publication. All perturbations and analysis have produced results very close
to the published experiments. The model was successfully tested on CoPaSi
v.4.4 (build 26).

Parameters not included in the publication:

1\. Parameters for SSAT kinetic constants:

KmAcCoA = 1.5 µM

KmCoA = 40 µM

2\. Parameters for equation MAT (table 1):

Vmax_MAT = 0.45 µM/min

Km_MAT = 41 µM

Ki_MET_MAT = 50 µM

3\. Erratum.: The corrected ODE for time-dependent variable Antz is:

KsANTZ*(1-1/(1+Keq*0.01*([D]+[S])))-KdANTZ*[Antz]

According to these modifications the new steady-state analysis results are:

Metabolites:

[P]= 104.681 µM

[D]= 76.7492 µM

[S]= 58.0135 µM

[SAM]= 52.327 µM

[A]= 0.0101962 µM

[aS]= 0.0245375 µM

[aD]= 0.832236 µM

Time-dependent global parameters:

[Antz] = 0.574038 µM

Vmaxodc = 1.28315 µM/min

Vmaxssat = 0.673814 µM/min

Vmaxsamdc = 0.36829 µM/min

  

To the extent possible under law, all copyright and related or neighbouring
rights to this encoded model have been dedicated to the public domain
worldwide. Please refer to [CC0 Public Domain
Dedication](http://creativecommons.org/publicdomain/zero/1.0/) for more
information.

In summary, you are entitled to use this encoded model in absolutely any
manner you deem suitable, verbatim, or with modification, alone or embedded it
in a larger context, redistribute it, commercially or not, in a restricted way
or not.

  

To cite BioModels Database, please use: [Li C, Donizelli M, Rodriguez N,
Dharuri H, Endler L, Chelliah V, Li L, He E, Henry A, Stefan MI, Snoep JL,
Hucka M, Le Novère N, Laibe C (2010) BioModels Database: An enhanced, curated
and annotated resource for published quantitative kinetic models. BMC Syst
Biol., 4:92.](http://www.ncbi.nlm.nih.gov/pubmed/20587024)


