# Mapping clinical risk estimates incorporating between-individual heterogeneity

## risk_transfer.ipynb  <br>
A code to map event risk estimates in event-free individuals from established AF populations (prevalent cohorts, from which risk scores were derived) to the same-aged, newly diagnosed AF populations (incident cohort).

####  Arguments: <br>
1) RR: prespecified relative risk (hazard ratio) of the history of prior events <br>
2) rate: aging rate (hazard ratio of age per year) <br>
3) latency and ref_T: time interval over which the average hazard ratio is calibrated to match the prespecified relative risk (RR). <br>
Parameters are determined so that the average relative risk over the interval [latency, ref_T] equals the prescribed RR. <br>

####  Frailty Distribution:  <br>
1) GammaFrailty: Use this class to specify a gamma frailty distribution. <br>
2) PVFFrailty: Use this class for other distributions in the PVF family (e.g., a = 0.5 for inverse Gaussian, and a < 0 for compound Poisson). <br>

## Caveat: <br>
This code provides theoretical predictions based on prescribed parameters and assumed frailty distributions. Users should exercise clinical judgment and consider all available information when making decisions.

## Reference: <br>
Tomoki Nakamizo, Munechika Misumi, Satoshi Kurisu, and Nobuo Sasaki. Are stroke risk scores safely applicable to newly diagnosed atrial fibrillation? available at https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5045986 

