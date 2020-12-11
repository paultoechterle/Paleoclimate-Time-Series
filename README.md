# Paleoclimate-Time-Series

## What is this?

The scripts herein chiefly use the output of an depth-age model (e.g. Oxcal) to plot time series proxy records including age uncertainties. 

The fundamental approach is taken from COPRA [1]:
The age uncertainty is obtained from multiple monte-carlo type depth-age model runs and expressed as a 95% confidence interval of possible ages per age interval. This uncertainty is then used to collect a sample of possible proxy values, that fall within this 95% age range based on the depth-age models' ensemble mean. A propability- (or alternatively a kernel-) density function can then be fitted to the sample of proxy values.
By iteratively repeating this fitting process to each time interval, a matrix of proxy propabilities can be generated, where each column represents the propability distribution of proxy values that arises from age uncertainty. In other words: the age uncertainty is projected onto the proxy axis.
[1] Breitenbach, S. F. M., Rehfeld, K., Goswami, B., Baldini, J. U. L., Ridley, H. E., Kennett, D. J., Prufer, K. M., Aquino, V. V., Asmerom, Y., Polyak, V. J., Cheng, H., Kurths, J., and Marwan, N.: COnstructing Proxy Records from Age models (COPRA), Clim. Past, 8, 1765–1779, https://doi.org/10.5194/cp-8-1765-2012
