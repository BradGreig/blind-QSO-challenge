# Overview

This page contains a summary of the blind QSO reconstruction project along with links to various data products. For further details refer to the main publication, Greig et al. (in prep).

On this page you can find the following:

- [Methodology](#methodology)
- [Reconstruction pipelines](#reconstruction-pipelines)
- [Individual profile reconstructions](#individual-profile-reconstructions)
- [Contact Information](#contact-information)

## Methodology

To test the performance of all (at the time) known QSO reconstruction pipelines at predicting the Lyman-alpha (Ly&alpha;) line profile (1180-1260&#8491;) from a small, unified sample of QSOs. For each QSO, the QSO flux was blinded (removed) prior to performing the QSO flux predictions. In total, 60 QSOs were reconstructed, with 30 QSOs each obtained from X-Shooter ([XQ-100](https://ui.adsabs.harvard.edu/abs/2016A&A...594A..91L)) and SDSS (BOSS [DR16](https://ui.adsabs.harvard.edu/abs/2020ApJS..250....8L)).

## Reconstruction pipelines

In total 9 different reconstruction pipelines were utilised for this comparison project. Below, a brief summary of each is provided along with links to the original publication.

- [Greig](https://ui.adsabs.harvard.edu/abs/2017MNRAS.466.1814G): Covariance matrix reconstruction based on the measured line-correlation strengths between Ly&alpha;, N V , C IV, Si IV + O IV doublet and C III obtained from a large training set of low-z QSOs. Line profiles are fit with a mixture of single and double component Gaussian profiles characterising the line width, height and velocity offset. 
- [Davies](https://ui.adsabs.harvard.edu/abs/2018ApJ...864..143D): Spectral decomposition of the QSO flux following principal component analysis (PCA). Predict the blue-side (<1280&#8491;) PCA components from the red-side components by applying a projection matrix trained on a low-z sample of QSOs.
- [QSANNdRA (&#270;urov&#269;&iacute;kov&aacute;)](https://ui.adsabs.harvard.edu/abs/2020MNRAS.493.4256D): An extension of the Davies approach, connecting the blue-red side PCA components with an artifical neural network (ANN). Consider a larger and new training set of QSOs along with more PCA components.
- [Fathivavsari](https://ui.adsabs.harvard.edu/abs/2020ApJ...898..114F): Neural network reconstruction of the QSO flux within each spectral bin between 1170-1290&#8491; based on the observed QSO flux around C IV, the Si IV + O IV doublet and C III.
- [Spectre (Reiman)](https://ui.adsabs.harvard.edu/abs/2020arXiv200600615R): An extension of QSANNdRA utilising normalising flows to provide a probabilistic distribution of reconstructed QSO profiles.
- [iQNet (Liu)](https://ui.adsabs.harvard.edu/abs/2021MNRAS.502.3510L): Simple auto encoder network to predict the Ly&alpha; flux based on redward information.
- [Bosman](https://ui.adsabs.harvard.edu/abs/2022ApJ...931...29C/abstract): An extension of the Davies PCA based reconstruction approach with a larger training set.
- [QFA (Sun)](https://ui.adsabs.harvard.edu/abs/2023ApJS..269....4S): unsupervised and probabilisitic reconstruction approach based on latent factor analysis.
- Meyer: An information maximising variational auto encoder is used to predict the Ly&alpha; profile based on the redward information.

## Individual profile reconstructions

Below, a table is provided containing the selected QSOs from X-Shooter (Sample 1) and SDSS/BOSS (Sample 2) along with link to a figure demonstrating the performance of each reconstruction pipeline.

#### Sample 1 (X-Shooter)

A compressed file containing all individual QSO reconstructions for this specific sample can be found [here](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Compressed/Dec7th_2023-Sample1.zip "download").


| QSO name | Redshift | Figure | | QSO name | Redshift | Figure |
| -------- | ------- | -------- | ------- | -------- | ------- | ------- |
| BR J0030-5159 | 4.17 | [Spectrum #1](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample1/Sample1_Spectrum1.pdf) | | J112617-012632 | 3.63 | [Spectrum #16](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample1/Sample1_Spectrum16.pdf) |
| HB89 0055-269 | 3.66 | [Spectrum #2](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample1/Sample1_Spectrum2.pdf) | | HB89 1159+123 | 3.52 | [Spectrum #17](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample1/Sample1_Spectrum17.pdf) |
| PMN J0100-2708 | 3.55 | [Spectrum #3](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample1/Sample1_Spectrum3.pdf) | | SDSSJ1202-0054 | 3.59 | [Spectrum #18](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample1/Sample1_Spectrum18.pdf) |
| PSS J0117+1552 | 4.24 | [Spectrum #4](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample1/Sample1_Spectrum4.pdf) | | J124837+130440 |3.72  | [Spectrum #19](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample1/Sample1_Spectrum19.pdf) |
| BR J0401-1711 | 4.23 | [Spectrum #5](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample1/Sample1_Spectrum5.pdf) | | J135247+130311 | 3.71 | [Spectrum #20](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample1/Sample1_Spectrum20.pdf) |
| BR J0529-3526 | 4.42 | [Spectrum #6](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample1/Sample1_Spectrum6.pdf) | | SDSSJ1416+1811 | 3.59 | [Spectrum #21](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample1/Sample1_Spectrum21.pdf) |
| SDSS J075552.41 | 3.67 | [Spectrum #7](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample1/Sample1_Spectrum7.pdf) | | PKS B1418-064 | 3.69 | [Spectrum #22](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample1/Sample1_Spectrum22.pdf) |
| SDSS J083322.50 | 3.72 | [Spectrum #8](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample1/Sample1_Spectrum8.pdf) | | J144250+092001 | 3.536 | [Spectrum #23](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample1/Sample1_Spectrum23.pdf) |
| SDSS J093714.48 | 3.70 | [Spectrum #9](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample1/Sample1_Spectrum9.pdf) | | SDSSJ1445+0958 | 3.56 | [Spectrum #24](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample1/Sample1_Spectrum24.pdf) |
| J101818+054822 | 3.52 | [Spectrum #10](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample1/Sample1_Spectrum10.pdf) | | J150328+041949 | 3.69 | [Spectrum #25](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample1/Sample1_Spectrum25.pdf) |
| BR 1033-0327 | 4.53 | [Spectrum #11](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample1/Sample1_Spectrum11.pdf) | | SDSSJ1517+0511 | 3.55 | [Spectrum #26](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample1/Sample1_Spectrum26.pdf) |
| SDSSJ1037+2135 | 3.63 | [Spectrum #12](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample1/Sample1_Spectrum12.pdf) | | J1621-0042 | 3.71 | [Spectrum #27](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample1/Sample1_Spectrum27.pdf) |
| SDSSJ1042+1957 | 3.63 | [Spectrum #13](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample1/Sample1_Spectrum13.pdf) | | PSS J1723+2243 | 4.53 | [Spectrum #28](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample1/Sample1_Spectrum28.pdf) |
| SDSS J105340.75| 3.66 | [Spectrum #14](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample1/Sample1_Spectrum14.pdf) | | J2239536-055219 | 4.56 | [Spectrum #29](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample1/Sample1_Spectrum29.pdf) |
| J111701+131115 | 3.62 | [Spectrum #15](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample1/Sample1_Spectrum15.pdf) | | BR 2248-1242 | 4.16 | [Spectrum #30](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample1/Sample1_Spectrum30.pdf) |

#### Sample 2 (BOSS/SDSS)

A compressed file containing all individual QSO reconstructions for this specific sample can be found [here](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Compressed/Dec7th_2023-Sample1.zip).

| QSO name | Redshift | Figure | | QSO name | Redshift | Figure |
| -------- | ------- | -------- | ------- | -------- | ------- | ------- |
| 3682-55244-942 | 3.76 | [Spectrum #1](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample2/Sample2_Spectrum1.pdf) | | 5184-56352-692 | 3.64 | [Spectrum #16](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample2/Sample2_Spectrum16.pdf) |
| 3776-55209-946 | 3.60 | [Spectrum #2](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample2/Sample2_Spectrum2.pdf) | | 5376-55987-382 | 3.69 | [Spectrum #17](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample2/Sample2_Spectrum17.pdf) |
| 3779-55222-358 | 3.63 | [Spectrum #3](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample2/Sample2_Spectrum3.pdf) | |  5443-56010-898 | 3.69 | [Spectrum #18](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample2/Sample2_Spectrum18.pdf) |
| 3839-55575-164 | 3.63 | [Spectrum #4](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample2/Sample2_Spectrum4.pdf) | | 5444-56038-798 | 3.68  | [Spectrum #19](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample2/Sample2_Spectrum19.pdf) |
| 3860-55269-816 | 3.63 | [Spectrum #5](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample2/Sample2_Spectrum5.pdf) | | 5472-55976-822 | 3.54 | [Spectrum #20](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample2/Sample2_Spectrum20.pdf) |
| 3872-55382-651 | 3.65 | [Spectrum #6](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample2/Sample2_Spectrum6.pdf) | | 5715-56657-890 | 3.97 | [Spectrum #21](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample2/Sample2_Spectrum21.pdf) |
| 4011-55635-724 | 3.60 | [Spectrum #7](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample2/Sample2_Spectrum7.pdf) | | 6418-56354-249 | 3.77 | [Spectrum #22](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample2/Sample2_Spectrum22.pdf) |
| 4178-55653-342 | 3.77 | [Spectrum #8](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample2/Sample2_Spectrum8.pdf) | | 6512-56567-682 | 3.93 | [Spectrum #23](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample2/Sample2_Spectrum23.pdf) |
| 4229-55501-552 | 3.84 | [Spectrum #9](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample2/Sample2_Spectrum9.pdf) | | 6713-56402-346 | 3.57 | [Spectrum #24](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample2/Sample2_Spectrum24.pdf) |
| 4361-55831-656 | 3.52 |[Spectrum #10](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample2/Sample2_Spectrum10.pdf) | | 6745-56425-330 | 3.83 | [Spectrum #25](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample2/Sample2_Spectrum25.pdf) |
| 4629-55630-210 | 3.95 | [Spectrum #11](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample2/Sample2_Spectrum11.pdf) | | 6758-56415-369 | 3.90 | [Spectrum #26](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample2/Sample2_Spectrum26.pdf) |
| 4711-55737-766 | 3.62 | [Spectrum #12](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample2/Sample2_Spectrum12.pdf) | | 7085-56625-895 | 3.77 | [Spectrum #27](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample2/Sample2_Spectrum27.pdf) |
| 4747-55652-761 | 3.66 | [Spectrum #13](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample2/Sample2_Spectrum13.pdf) | | 7096-56683-885 | 3.69 | [Spectrum #28](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample2/Sample2_Spectrum28.pdf) |
| 4799-55656-446 | 4.11 | [Spectrum #14](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample2/Sample2_Spectrum14.pdf) | | 7112-56666-380 | 3.52 | [Spectrum #29](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample2/Sample2_Spectrum29.pdf) |
| 5174-56047-750 | 3.55 | [Spectrum #15](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample2/Sample2_Spectrum15.pdf) | | 9616-58135-682 | 4.02 | [Spectrum #30](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample2/Sample2_Spectrum30.pdf) |

## Contact Information

For any questions please contact [Brad Greig](mailto:brad.s.greig@gmail.com).