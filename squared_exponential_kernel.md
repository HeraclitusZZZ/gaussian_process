# Squared Exponential Kernel

![This is an image](./sek.svg)

where &sigma;<sup>2</sup> is the signal variance, l>0 is the lengthscale and &sigma;<sub>noise</sub><sup>2</sup>&geq;0 is the noise variance. The noise variance is applied only when i=j.

Squared exponential is appropriate for modelling very smooth functions. The parameters have the following interpretation:

- **Lengthscale** l describes how smooth a function is. Small lengthscale value means that function values can change quickly, large values characterize f

small lengthscale

![This is an image](./smallLengthscale.png)

large lengthscale

![This is an image](./largeLengthscale.png)

- **Signal variance** &sigma;<sup>2</sup> is a scaling factor. It determines variation of function values from their mean. Small value of &sigma;<sup>2</sup> characterize functions that stay close to their mean value, larger values allow more variation. If the signal variance is too large, the modelled function will be free to chase outliers.

small signal variance

![This is an image](./smallSignalVariance.png)

large signal variance

![This is an image](./largeSignalVariance.png)

- **Noise variance** &sigma;<sub>noise</sub><sup>2</sup> is formally not a part of the covariance function itself. It is used by the Gaussian process model to allow for noise present in training data. This parameter specifies how much noise is expected to be present in the data.

small noise variance

![This is an image](./smallNoiseVariance.png)

large noise variance

![This is an image](./largeNoiseVariance.png)

## Reference

[1] http://evelinag.com/Ariadne/covarianceFunctions.html
