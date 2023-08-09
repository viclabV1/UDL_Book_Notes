These [[Model]]s learn to map from [[Input]] data to an [[Output]] [[Prediction]].

The actual computation of the output from the input is [[Inference]]
The [[Model]] itself is a mathematical equation with multiple [[Parameter]]s.

[[Regression]]
[[Classification]]

Supervised models can benefit from some [[Unsupervised Learning]]. Especially useful when the [[Output]] data has structure. 
Ex: If there was a system that predicted the image that was described by a caption, it might be better to represent both the [[Input]] text and [[Output]] images using [[Latent Variables]], so that the relationship learned is between these latent variables rather than between the text and image directly.
There are three advantages to this:
1) Less [[Training Data]] may be needed as the data now has a lower [[Dimension]].
2) More likely to generate a plausible looking image.
3) By introducing randomness to either the mapping between the two sets of latent variables or the mapping from the latent variables to the image, multiple images can be generated from one caption. 

#### Math

The goal is to define a [[Model]]/function $f$ that will take the [[Input]] $x$ and give the [[Output]] $y$. Here, **x** and **y** are understood to be vectors of a predetermined and constant [[Size]] and of a constant order (structured/[[Tabular Data]]).
$$
y=f[x]
$$
The computation of this equation is [[Inference]]. The model also has [[Parameter]]s $\phi$. 
$$
y=f[x,\phi]
$$
[[Training]] is the adjustment of $\phi$ such that [[Loss]] function $L[\phi]$ is minimized on [[Input]]/[[Output]] pairs $\{x_i, y_i\}$. The result of training will be the optimized [[Parameter]]s $\hat{\phi}$. 
$$
\hat{\phi}=\underset{\phi}{argmin}[L[\phi]]
$$
After [[Training]], good idea to [[Test]] the [[Performance]] of the [[Model]] on [[Test Data]] to see how well it generalizes([[Generalization]]) on data not in the [[Training Data]].