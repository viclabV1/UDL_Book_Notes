These models learn to map from [[Input]] data to an [[Output]] [[Prediction]].

[[Regression]]
[[Classification]]

Supervised models can benefit from some [[Unsupervised Learning]]. Especially useful when the [[Output]] data has structure. 
Ex: If there was a system that predicted the image that was described by a caption, it might be better to represent both the [[Input]] text and [[Output]] images using [[Latent Variables]], so that the relationship learned is between these latent variables rather than between the text and image directly.
There are three advantages to this:
1) Less [[Training Data]] may be needed as the data now has a lower [[Dimension]].
2) More likely to generate a plausible looking image.
3) By introducing randomness to either the mapping between the two sets of latent variables or the mapping from the latent variables to the image, multiple images can be generated from one caption. 