# Overview

This page contains a summary of the blind QSO reconstruction project along with links to various data products. For further details refer to the main publication, Greig et al. (in prep).

On this page you can find the following:

- [Methodology](#methodology)
- [Reconstruction pipelines](#reconstruction-pipelines)
- [Individual profile reconstructions](#individual-reconstructions)
- [Contact Information](#contact-information)

## Methodology

To test the performance of all (at the time) known QSO reconstruction pipelines at predicting the Lyman-alpha (Ly&alpha;) line profile (1180-1260&#8491;) from a small, unified sample of QSOs. For each QSO, the QSO flux was blinded (removed) prior to performing the QSO flux predictions. In total, 60 QSOs were reconstructed, with 30 QSOs each obtained from X-Shooter ([XQ-100](https://ui.adsabs.harvard.edu/abs/2016A&A...594A..91L)) and SDSS (BOSS [DR16](https://ui.adsabs.harvard.edu/abs/2020ApJS..250....8L)).

## Reconstruction pipelines

In total 9 different reconstruction pipelines were utilised for this comparison project. Below, a brief summary of each is provided along with links to the original publication.

- [Greig](https://ui.adsabs.harvard.edu/abs/2017MNRAS.466.1814G): Covariance matrix reconstruction based on the measured line-correlation strengths between Ly&alpha;, N\,{\scriptsize V}, CIV, Si IV + O IV and CIII obtained from a large training set of low-z QSOs 
- [Davies](https://ui.adsabs.harvard.edu/abs/2018ApJ...864..143D): 
- [QSANNdRA ({{\v{D}}urov{\v{c}}{\'\i}kov{\'a})](https://ui.adsabs.harvard.edu/abs/2020MNRAS.493.4256D):
- [Fathivavsari](https://ui.adsabs.harvard.edu/abs/2020ApJ...898..114F)
- [Spectre (Reiman)](https://ui.adsabs.harvard.edu/abs/2020arXiv200600615R):
- [iQNet (Liu)](https://ui.adsabs.harvard.edu/abs/2021MNRAS.502.3510L):
- [Bosman](https://ui.adsabs.harvard.edu/abs/2022ApJ...931...29C/abstract):
- [QFA (Sun)](https://ui.adsabs.harvard.edu/abs/2023ApJS..269....4S):

## Individual profile reconstructions

#### Sample 1 (X-Shooter)

| QSO name | Redshift | Figure | | QSO name | Redshift | Figure |
| -------- | ------- | -------- | ------- | -------- | ------- | ------- |
| BR J0030-5159 | 4.17 | Spectrum #1 | | J112617-012632 | 3.63 | Spectrum #16 |
| HB89 0055-269 | 3.66 | Spectrum #2 | | HB89 1159+123 | 3.52 | Spectrum #17 |
| PMN J0100-2708 | 3.55 | [Spectrum #3](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample1/Sample1_Spectrum3.pdf) | | SDSSJ1202-0054 | 3.59 | Spectrum #18 |
| PSS J0117+1552 | 4.24 | [Spectrum #4](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample1/Sample1_Spectrum4.pdf) | | J124837+130440 |3.72  | Spectrum #19 |
| BR J0401-1711 | 4.23 | Spectrum #5 | | J135247+130311 | 3.71 | Spectrum #20 |
| BR J0529-3526 | 4.42 | Spectrum #6 | | SDSSJ1416+1811 | 3.59 | Spectrum #21 |
| SDSS J075552.41 | 3.67 | Spectrum #7 | | PKS B1418-064 | 3.69 | Spectrum #22 |
| SDSS J083322.50 | 3.72 | Spectrum #8 | | J144250+092001 | 3.536 | Spectrum #23 |
| SDSS J093714.48 | 3.70 | Spectrum #9 | | SDSSJ1445+0958 | 3.56 | Spectrum #24 |
| J101818+054822 | 3.52 | Spectrum #10 | | J150328+041949 | 3.69 | Spectrum #25 |
| BR 1033-0327 | 4.53 | Spectrum #11 | | SDSSJ1517+0511 | 3.55 | Spectrum #26 |
| SDSSJ1037+2135 | 3.63 | Spectrum #12 | | J1621-0042 | 3.71 | Spectrum #27 |
| SDSSJ1042+1957 | 3.63 | Spectrum #13 | | PSS J1723+2243 | 4.53 | Spectrum #28 |
| SDSS J105340.75| 3.66 | Spectrum #14 | | J2239536-055219 | 4.56 | Spectrum #29 |
| J111701+131115 | 3.62 | Spectrum #15 | | BR 2248-1242 | 4.16 | Spectrum #30 |

#### Sample 2 (BOSS/SDSS)

| QSO name | Redshift | Figure | | QSO name | Redshift | Figure |
| -------- | ------- | -------- | ------- | -------- | ------- | ------- |
| 3682-55244-942 | 3.76 | Spectrum #1 | | 5184-56352-692 | 3.64 | [Spectrum #16](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample2/Sample2_Spectrum16.pdf) |
| 3776-55209-946 | 3.60 | Spectrum #2 | | 5376-55987-382 | 3.69 | Spectrum #17 |
| 3779-55222-358 | 3.63 | Spectrum #3 | |  5443-56010-898 | 3.69 | Spectrum #18 |
| 3839-55575-164 | 3.63 | Spectrum #4 | | 5444-56038-798 | 3.68  | Spectrum #19 |
| 3860-55269-816 | 3.63 | Spectrum #5 | | 5472-55976-822 | 3.54 | Spectrum #20 |
| 3872-55382-651 | 3.65 | Spectrum #6 | | 5715-56657-890 | 3.97 | Spectrum #21 |
| 4011-55635-724 | 3.60 | Spectrum #7 | | 6418-56354-249 | 3.77 | Spectrum #22 |
| 4178-55653-342 | 3.77 | Spectrum #8 | | 6512-56567-682 | 3.93 | Spectrum #23 |
| 4229-55501-552 | 3.84 | Spectrum #9 | | 6713-56402-346 | 3.57 | Spectrum #24 |
| 4361-55831-656 | 3.52 | Spectrum #10 | | 6745-56425-330 | 3.83 | [Spectrum #25](https://github.com/BradGreig/blind-QSO-challenge/blob/main/data/Sample2/Sample2_Spectrum25.pdf) |
| 4629-55630-210 | 3.95 | Spectrum #11 | | 6758-56415-369 | 3.90 | Spectrum #26 |
| 4711-55737-766 | 3.62 | Spectrum #12 | | 7085-56625-895 | 3.77 | Spectrum #27 |
| 4747-55652-761 | 3.66 | Spectrum #13 | | 7096-56683-885 | 3.69 | Spectrum #28 |
| 4799-55656-446 | 4.11 | Spectrum #14 | | 7112-56666-380 | 3.52 | Spectrum #29 |
| 5174-56047-750 | 3.55 | Spectrum #15 | | 9616-58135-682 | 4.02 | Spectrum #30 |

## Contact Information

For any questions please contact [Brad Greig](mailto:brad.s.greig@gmail.com).