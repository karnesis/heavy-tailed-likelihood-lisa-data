## Characterization of non-Gaussian stochastic signals with heavier-tailed likelihoods

This is a repository supporting the publication of [[2410.14354](https://arxiv.org/abs/2410.14354)], which is accepted for publication to Phys. Rev. D.

By N. Karnesis, A. Sasli, R. Buscicchio, N. Stergioulas

This work develops a robust statistical framework for parameter estimation of stochastic signals. This framework is based on the hyperbolic distribution [[2305.04709](https://arxiv.org/abs/2305.04709)]. The hyperbolic likelihood can be used to perform parameter estimation of the signal, and at the same time detect any departures from Gaussianities. 

In order to demonstrate the capabilities of such framework, we have generated synthetic data of the future [LISA mission](https://www.esa.int/Science_Exploration/Space_Science/LISA_factsheet). The data contain Gravitational Wave signals emmitted by the $$\mathcal{O}(10^7)$$ Double White Dwarf binaries in our Galaxy. 

You can download the data (in `h5` format) using [this link](http://data.physics.auth.gr/heavier_tailed_likelihood/ucb_signal_lisa.h5).

The data contain the signal time-series in the noise-orthogonal Time Delay Interferometer channels A, E, and T. You can load the data as
```
import pandas as pd
data = pd.read_hdf("ucb_signal_lisa.h5")
```
And printing the output should look like the below
```
In [3]: data
Out[3]:
         TDI Channel 1  TDI Channel 2  TDI Channel 3       Time
0         2.268757e-23  -1.059437e-23   3.189122e-27          0
1         2.209987e-23  -2.266132e-23   3.316861e-27         15
...                ...            ...            ...        ...
8399997  -2.398883e-23   3.031537e-23   4.153636e-27  125999955
8399998  -2.510490e-23   1.912378e-23   4.579830e-27  125999970
8399999  -2.638566e-23   5.883557e-24   4.685575e-27  125999985

[8400000 rows x 4 columns]
```

You can cite this work using the bibtex item below:
```
@article{Karnesis:2024pxh,
    author = "Karnesis, Nikolaos and Sasli, Argyro and Buscicchio, Riccardo and Stergioulas, Nikolaos",
    title = "{Characterization of non-Gaussian stochastic signals with heavier-tailed likelihoods}",
    eprint = "2410.14354",
    archivePrefix = "arXiv",
    primaryClass = "gr-qc",
    month = "10",
    year = "2024"
}
```
