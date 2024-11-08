#### IGNORE REPORT3, GO STRAIGHT TO REPORT 3 (2)

#### Introduction
In this report I applied SVM models with polynomial and RBF kernels to two different non-linear datasets: the make_moons dataset and the spiral dataset. The goal was to evaluate the performance of these kernels in capturing non-linear decision boundaries. 

#### Methods
The make_moons dataset consists of two cresent shaped classes with 200 samples in total. 
The spiral dataset consists of two intertwined spirals with 200 samples in total. 

Polynomial Kernel:
<br>
The polynomial kernel maps the data into a higher-dimensional space using polynomial functions.
<br>
The formula for the polynomial kernel is:
<br>
$K(x, x') = (γ \cdot [x, x'] + coefO)^{degree}$
<br>
where:
<br>
γ is a scaling parameter 
<br>
coef0 is a constant to control the influence of higher-order terms
<br>
degree is the degree of the polynomial kernel.

RBF (Gaussian) Kernel:
<br>
The RBF kernel maps the data into an infinite-dimensional feature space.
<br>
The formula for the RBF kernel is:
<br>
$K(x, x') = exp(-γ||x-x'||^{degree})$
<br>
where:
<br>
γ is a parameter that defines the width of the Gaussian function.

#### Results
Both kernels performed well on the make_moons dataset, with the polynomial kernel slightly outperforming the RBF kernel. On the spiral dataset, however, the performance gap between the two kernels was more pronounced, with the polynomial kernel outperforming the RBF kernel by a considerable margin.
This suggests that the polynomial kernel works best when the data is well-behaved like the make_moons dataset but may struggle with more complex datasets like spiral while the RBF kernel is more flexible but may need tuning of the 𝛾 parameter. 


