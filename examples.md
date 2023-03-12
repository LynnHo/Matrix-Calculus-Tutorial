<h1> Examples </h1>

<!-- MarkdownTOC -->

- [1. Practical Examples](#1-practical-examples)
- [2. Special Examples](#2-special-examples)

<!-- /MarkdownTOC -->

## 1. Practical Examples

**E.g. 1**, Deriving PCA by minimizing MSE

- <img src="svg/684d1346c74b9987de0c17d9c53cf2ac.svg?invert_in_darkmode" align=middle width=203.00764604999998pt height=24.65753399999998pt/>, <img src="svg/c416d0c6d8ab37f889334e2d1a9863c3.svg?invert_in_darkmode" align=middle width=14.628015599999989pt height=14.611878600000017pt/> is the <img src="svg/77a3b857d53fb44e33b53e4c8b68351a.svg?invert_in_darkmode" align=middle width=5.663225699999989pt height=21.68300969999999pt/>-th sample with m dimension. Assume for simplicity that <img src="svg/d05b996d2c08252f77613c25205a0f04.svg?invert_in_darkmode" align=middle width=14.29216634999999pt height=22.55708729999998pt/> has zero mean.
- <img src="svg/805f1ba29a4965179d1766344a78003f.svg?invert_in_darkmode" align=middle width=217.82867865pt height=24.65753399999998pt/>, <img src="svg/831047ac6f850b0d588c94d84fc6f4c1.svg?invert_in_darkmode" align=middle width=19.75740524999999pt height=14.611878600000017pt/> is the <img src="svg/36b5afebdba34564d884d347484ac0c7.svg?invert_in_darkmode" align=middle width=7.710416999999989pt height=21.68300969999999pt/>-th basis vector with m dimension.
- <img src="svg/c053a97af423085b0d1caff7bad21361.svg?invert_in_darkmode" align=middle width=266.19297209999996pt height=27.91243950000002pt/>, <img src="svg/9fb01b1f049f71510ce5c71a29044cc5.svg?invert_in_darkmode" align=middle width=82.89732165pt height=27.91243950000002pt/> is the low dimension representation of <img src="svg/c416d0c6d8ab37f889334e2d1a9863c3.svg?invert_in_darkmode" align=middle width=14.628015599999989pt height=14.611878600000017pt/>.

The optimization problem of PCA is

<p align="center"><img src="svg/29c78824c7a61b548ec04ab6d9565e59.svg?invert_in_darkmode" align=middle width=649.1553024pt height=82.98738359999999pt/></p>

We can simplify the above problem by using <img src="svg/5c1be6a2e2ad9f7bc05cc2b96913e716.svg?invert_in_darkmode" align=middle width=407.3047274999999pt height=27.91243950000002pt/> and <img src="svg/a5d4fd403c305234001f2f87d133519b.svg?invert_in_darkmode" align=middle width=79.79416499999999pt height=27.91243950000002pt/>, as

<p align="center"><img src="svg/1f80db88a38606d519d5360fe87c5722.svg?invert_in_darkmode" align=middle width=177.6595425pt height=78.8777946pt/></p>

Introducing the Lagrange multipliers <img src="svg/15c6364fc6c8a9ac330de3cc1dd76297.svg?invert_in_darkmode" align=middle width=108.05943059999998pt height=24.65753399999998pt/> and <img src="svg/3a4921573f3ddd88fef975e48b03fb34.svg?invert_in_darkmode" align=middle width=108.05943059999998pt height=24.65753399999998pt/>, the optimization problem is equivalent to

<p align="center"><img src="svg/8ac1adc2cab49704bbd30386e8dbce6e.svg?invert_in_darkmode" align=middle width=643.57777275pt height=57.95347964999999pt/></p>

where we use <img src="svg/d37fd43b0bbbbbf3e43cf14bc25fa23f.svg?invert_in_darkmode" align=middle width=172.41955334999997pt height=27.91243950000002pt/>, and let <img src="svg/418646bd58f82cd21db79833604153d8.svg?invert_in_darkmode" align=middle width=155.80308315pt height=24.7161288pt/>.

***Next***, we will derive <img src="svg/812ea914ddbd5c7b8de749d8e906a6f8.svg?invert_in_darkmode" align=middle width=23.155842599999996pt height=28.92634470000001pt/>.

<p align="center"><img src="svg/def613611f4a6de062366f4d4ffb468f.svg?invert_in_darkmode" align=middle width=747.00524745pt height=127.9730364pt/></p>

Therefore <img src="svg/c5aef706035e4c1858fd5dd2c833d7dd.svg?invert_in_darkmode" align=middle width=427.78704045pt height=28.92634470000001pt/>. Let it be <img src="svg/60eb568c0573744ea49707553106a93f.svg?invert_in_darkmode" align=middle width=9.452005199999991pt height=21.18721440000001pt/>, we get

<p align="center"><img src="svg/964bf31ee86abec2555f40e2fdf2fc46.svg?invert_in_darkmode" align=middle width=319.67028719999996pt height=36.35277855pt/></p>

Left multiply the equation by <img src="svg/9e8ffed85b9290db84ba5b6f98e56762.svg?invert_in_darkmode" align=middle width=30.07986959999999pt height=27.91243950000002pt/> and use eq. (2) - <img src="svg/a5d4fd403c305234001f2f87d133519b.svg?invert_in_darkmode" align=middle width=79.79416499999999pt height=27.91243950000002pt/> and eq. (3) - <img src="svg/9b0ceed0bf10a076c6acc03793081cf3.svg?invert_in_darkmode" align=middle width=187.61789639999998pt height=27.91243950000002pt/>, we get

<p align="center"><img src="svg/4881c708375c2ac17b4f37d280a28c13.svg?invert_in_darkmode" align=middle width=634.44980115pt height=74.0239665pt/></p>

from which we can see ***<img src="svg/47c91d5b4bf88dfbe2233a1b27bb8cbe.svg?invert_in_darkmode" align=middle width=15.693592199999989pt height=22.831056599999986pt/> is the eigenvalue of <img src="svg/a4ae53a03eecebede446b3cdc5eb7183.svg?invert_in_darkmode" align=middle width=38.85835304999999pt height=27.91243950000002pt/> and <img src="svg/831047ac6f850b0d588c94d84fc6f4c1.svg?invert_in_darkmode" align=middle width=19.75740524999999pt height=14.611878600000017pt/> is the corresponding eigenvector***.

Substitute eq. (4) into eq. (1),

<p align="center"><img src="svg/446ec8bf533862f656801999abf8ea01.svg?invert_in_darkmode" align=middle width=435.77233755pt height=149.10353865pt/></p>

therefore ***<img src="svg/ce9b0d1765717c60b7915f2a48951a92.svg?invert_in_darkmode" align=middle width=16.141629899999987pt height=22.831056599999986pt/>, <img src="svg/22d952fd172ae91ac1817c8f2b3be088.svg?invert_in_darkmode" align=middle width=16.141629899999987pt height=22.831056599999986pt/>, ..., <img src="svg/0c99b2af0fc5f8b1a39c8902837934f4.svg?invert_in_darkmode" align=middle width=16.855112999999992pt height=22.831056599999986pt/> should be the largest k eigenvalues***. <img src="svg/bcf9035465fb0a2d380bb9fc8c9d2545.svg?invert_in_darkmode" align=middle width=12.785434199999989pt height=22.19178720000002pt/>



## 2. Special Examples

**E.g. 1**, <img src="svg/ca960af172ffc76bd9f26a4be5e26ace.svg?invert_in_darkmode" align=middle width=63.6150108pt height=33.20539859999999pt/>, where <img src="svg/d05b996d2c08252f77613c25205a0f04.svg?invert_in_darkmode" align=middle width=14.29216634999999pt height=22.55708729999998pt/> is a <img src="svg/6751b03b5f3d6d66a90def3339c879c8.svg?invert_in_darkmode" align=middle width=36.28986404999999pt height=19.1781018pt/> matrix

<p align="center"><img src="svg/a004f1e62426b63737ecc8c87aa28719.svg?invert_in_darkmode" align=middle width=293.33587305pt height=532.17125775pt/></p>

or

<p align="center"><img src="svg/2211dff6fd22e1740aa0d3c5d1505f08.svg?invert_in_darkmode" align=middle width=351.38692215pt height=465.51294075pt/></p>

In the above, we haven't used any differential technique, because we haven't defined the derivative of vector-by-matrix <img src="svg/4cd51c073dc2f63ed2a687aabdf9e3c2.svg?invert_in_darkmode" align=middle width=17.980054949999996pt height=30.648287999999997pt/> which could be a 3D tensor. However, in some cases such as <img src="svg/fd6a90714b41269dcf4d29fd283b2fc5.svg?invert_in_darkmode" align=middle width=61.67770949999999pt height=22.55708729999998pt/> (w.r.t. <img src="svg/380c103b60c66d6420ec8923cdc6e6e8.svg?invert_in_darkmode" align=middle width=19.80585089999999pt height=22.55708729999998pt/>), the differential technique still works (see [this example](./README.md#y=Wx)).

**E.g. 2**, <img src="svg/8549adb88bfe36130ebab8cf4798e2e8.svg?invert_in_darkmode" align=middle width=67.05929834999999pt height=33.20539859999999pt/>, where <img src="svg/319d907db67f3000780e9b2d1a2816d9.svg?invert_in_darkmode" align=middle width=14.764759349999988pt height=22.55708729999998pt/> is a <img src="svg/63b142315f480db0b3ff453d62cc3e7f.svg?invert_in_darkmode" align=middle width=44.39116769999999pt height=19.1781018pt/> matrix and <img src="svg/d05b996d2c08252f77613c25205a0f04.svg?invert_in_darkmode" align=middle width=14.29216634999999pt height=22.55708729999998pt/> is a <img src="svg/6751b03b5f3d6d66a90def3339c879c8.svg?invert_in_darkmode" align=middle width=36.28986404999999pt height=19.1781018pt/> matrix

<p align="center"><img src="svg/a6f513ee10f611fd18a07a55e85d0ef3.svg?invert_in_darkmode" align=middle width=553.9515267pt height=625.9342254pt/></p>

In the above, we haven't used any differential technique, because we haven't defined the derivative of matrix-by-matrix <img src="svg/67f5bf892d3a85e4355fafecc13c8d5c.svg?invert_in_darkmode" align=middle width=18.347874599999994pt height=28.92634470000001pt/> which could be a 4D tensor. However, in some cases such as <img src="svg/20f8bd7d5b5393263f338e8c2a18b2cf.svg?invert_in_darkmode" align=middle width=65.26671524999999pt height=22.55708729999998pt/>, the differential technique still works (see [this example](./README.md#Y=AX)). Besides, there is another excellent example of <img src="svg/8549adb88bfe36130ebab8cf4798e2e8.svg?invert_in_darkmode" align=middle width=67.05929834999999pt height=33.20539859999999pt/>: derivative of SVD - https://arxiv.org/pdf/1509.07838.pdf.