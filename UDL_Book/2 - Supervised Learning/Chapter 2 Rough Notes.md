
### Sections
(First few sections were not written as rough notes)

#### 2.2 Linear Regression Example
##### 2.2.1 1D Linear Regression Example
$$
y = f[x,\phi] = \phi_0+\phi_1x_1
$$
the [[Prediction]] y is really just the [[Output]] given the [[Weight]]s as [[Input]](which can just be thought of as slope and y-intercept in slope-intercept form)

Parameters written as $\phi=[\phi_0,\phi_1]^T$ for some reason.
##### 2.2.2 [[Loss]]
|  |l
|| |_
how off prediction is from what we want prediction to be
in this case loss is the sum of the distances of each prediction from what prediction should be

$$
L[\phi]=\sum_{i=1}^I(f[x_i,\phi]-y_i)^2=\sum_{i=1}^I(\phi_0+\phi_1x_1-y_i)^2
$$
$$
\text{Where I is the total number of training pairs and i is the index of a pair.}
$$

Optimal [[Paramater]]s minimize, so this is a least-squares [[Loss]]. Loss function can be visualized as a surface (tb to [[Gradient Descent]])
[[Loss]] function also known as cost function

### Topics
[[Supervised Learning]] 
[[Model]]
[[Inference]]
[[Parameter]]
[[Training]]
[[Training Data]]
[[Loss]]
[[Generalization]]
[[Vector]]

