<h1> Examples </h1>

<!-- MarkdownTOC -->

- [1. Actual Examples](#1-actual-examples)
- [2. Abstract Examples](#2-abstract-examples)

<!-- /MarkdownTOC -->

## 1. Actual Examples

**E.g. 1** Deriving PCA by minimizing MSE.

- <img src="/tex/684d1346c74b9987de0c17d9c53cf2ac.svg?invert_in_darkmode&sanitize=true" align=middle width=203.00764604999998pt height=24.65753399999998pt/>, <img src="/tex/c416d0c6d8ab37f889334e2d1a9863c3.svg?invert_in_darkmode&sanitize=true" align=middle width=14.628015599999989pt height=14.611878600000017pt/> is the <img src="/tex/77a3b857d53fb44e33b53e4c8b68351a.svg?invert_in_darkmode&sanitize=true" align=middle width=5.663225699999989pt height=21.68300969999999pt/>-th sample with m dimension.
- <img src="/tex/805f1ba29a4965179d1766344a78003f.svg?invert_in_darkmode&sanitize=true" align=middle width=217.82867865pt height=24.65753399999998pt/>, <img src="/tex/831047ac6f850b0d588c94d84fc6f4c1.svg?invert_in_darkmode&sanitize=true" align=middle width=19.75740524999999pt height=14.611878600000017pt/> is the <img src="/tex/36b5afebdba34564d884d347484ac0c7.svg?invert_in_darkmode&sanitize=true" align=middle width=7.710416999999989pt height=21.68300969999999pt/>-th basis vector with m dimension.
- <img src="/tex/c053a97af423085b0d1caff7bad21361.svg?invert_in_darkmode&sanitize=true" align=middle width=266.19297209999996pt height=27.91243950000002pt/>, <img src="/tex/9fb01b1f049f71510ce5c71a29044cc5.svg?invert_in_darkmode&sanitize=true" align=middle width=82.89732165pt height=27.91243950000002pt/> is the low dimension representation of <img src="/tex/c416d0c6d8ab37f889334e2d1a9863c3.svg?invert_in_darkmode&sanitize=true" align=middle width=14.628015599999989pt height=14.611878600000017pt/>.

The optimization problem of PCA is,

<p align="center"><img src="/tex/141baf8e60a327f5c4cd6adf1789ac6b.svg?invert_in_darkmode&sanitize=true" align=middle width=650.67738615pt height=82.98738359999999pt/></p>

We can simplify the above problem by using <img src="/tex/18e3e1eadbf0c79931951f0e3b04a493.svg?invert_in_darkmode&sanitize=true" align=middle width=400.91201039999993pt height=27.91243950000002pt/> and <img src="/tex/a5d4fd403c305234001f2f87d133519b.svg?invert_in_darkmode&sanitize=true" align=middle width=79.79416499999999pt height=27.91243950000002pt/>, as

<p align="center"><img src="/tex/1f80db88a38606d519d5360fe87c5722.svg?invert_in_darkmode&sanitize=true" align=middle width=177.6595425pt height=78.8777946pt/></p>

Introducing the Lagrange multipliers <img src="/tex/15c6364fc6c8a9ac330de3cc1dd76297.svg?invert_in_darkmode&sanitize=true" align=middle width=108.05943059999998pt height=24.65753399999998pt/> and <img src="/tex/3a4921573f3ddd88fef975e48b03fb34.svg?invert_in_darkmode&sanitize=true" align=middle width=108.05943059999998pt height=24.65753399999998pt/>, the optimization problem is equivalent to

<p align="center"><img src="/tex/8ac1adc2cab49704bbd30386e8dbce6e.svg?invert_in_darkmode&sanitize=true" align=middle width=643.57777275pt height=57.95347964999999pt/></p>

where we use <img src="/tex/d37fd43b0bbbbbf3e43cf14bc25fa23f.svg?invert_in_darkmode&sanitize=true" align=middle width=172.41955334999997pt height=27.91243950000002pt/>, and let <img src="/tex/418646bd58f82cd21db79833604153d8.svg?invert_in_darkmode&sanitize=true" align=middle width=155.80308315pt height=24.7161288pt/>.

***Next***, we will derive <img src="/tex/812ea914ddbd5c7b8de749d8e906a6f8.svg?invert_in_darkmode&sanitize=true" align=middle width=23.155842599999996pt height=28.92634470000001pt/>.

<p align="center"><img src="/tex/0e3da11605f97b2463dc4efd789ed87d.svg?invert_in_darkmode&sanitize=true" align=middle width=747.00524745pt height=127.9730364pt/></p>

Therefore <img src="/tex/c5aef706035e4c1858fd5dd2c833d7dd.svg?invert_in_darkmode&sanitize=true" align=middle width=427.78704045pt height=28.92634470000001pt/>. Let it be <img src="/tex/60eb568c0573744ea49707553106a93f.svg?invert_in_darkmode&sanitize=true" align=middle width=9.452005199999991pt height=21.18721440000001pt/>, we get,

<p align="center"><img src="/tex/964bf31ee86abec2555f40e2fdf2fc46.svg?invert_in_darkmode&sanitize=true" align=middle width=319.67028719999996pt height=36.35277855pt/></p>

Left multiply the equation by <img src="/tex/9e8ffed85b9290db84ba5b6f98e56762.svg?invert_in_darkmode&sanitize=true" align=middle width=30.07986959999999pt height=27.91243950000002pt/> and use eq. (2): <img src="/tex/a5d4fd403c305234001f2f87d133519b.svg?invert_in_darkmode&sanitize=true" align=middle width=79.79416499999999pt height=27.91243950000002pt/>, and eq. (3): <img src="/tex/48652b7742e9c59e9a2dd45a4489e3ce.svg?invert_in_darkmode&sanitize=true" align=middle width=165.43769715pt height=27.91243950000002pt/>, we get

<p align="center"><img src="/tex/4881c708375c2ac17b4f37d280a28c13.svg?invert_in_darkmode&sanitize=true" align=middle width=634.44980115pt height=74.0239665pt/></p>

from which we can see ***<img src="/tex/47c91d5b4bf88dfbe2233a1b27bb8cbe.svg?invert_in_darkmode&sanitize=true" align=middle width=15.693592199999989pt height=22.831056599999986pt/> is the eigenvalue of <img src="/tex/a4ae53a03eecebede446b3cdc5eb7183.svg?invert_in_darkmode&sanitize=true" align=middle width=38.85835304999999pt height=27.91243950000002pt/> and <img src="/tex/831047ac6f850b0d588c94d84fc6f4c1.svg?invert_in_darkmode&sanitize=true" align=middle width=19.75740524999999pt height=14.611878600000017pt/> is the corresponding eigenvector***.

Substitute eq. (4) into eq. (1),

<p align="center"><img src="/tex/446ec8bf533862f656801999abf8ea01.svg?invert_in_darkmode&sanitize=true" align=middle width=435.77233755pt height=149.10353865pt/></p>

therefore ***<img src="/tex/ce9b0d1765717c60b7915f2a48951a92.svg?invert_in_darkmode&sanitize=true" align=middle width=16.141629899999987pt height=22.831056599999986pt/>, <img src="/tex/22d952fd172ae91ac1817c8f2b3be088.svg?invert_in_darkmode&sanitize=true" align=middle width=16.141629899999987pt height=22.831056599999986pt/>, ..., <img src="/tex/0c99b2af0fc5f8b1a39c8902837934f4.svg?invert_in_darkmode&sanitize=true" align=middle width=16.855112999999992pt height=22.831056599999986pt/> should be the largest k eigenvalues***. <img src="/tex/bcf9035465fb0a2d380bb9fc8c9d2545.svg?invert_in_darkmode&sanitize=true" align=middle width=12.785434199999989pt height=22.19178720000002pt/>



## 2. Abstract Examples

**E.g. 1**, <img src="/tex/ca960af172ffc76bd9f26a4be5e26ace.svg?invert_in_darkmode&sanitize=true" align=middle width=63.6150108pt height=33.20539859999999pt/>, (<img src="/tex/d05b996d2c08252f77613c25205a0f04.svg?invert_in_darkmode&sanitize=true" align=middle width=14.29216634999999pt height=22.55708729999998pt/> is a <img src="/tex/6751b03b5f3d6d66a90def3339c879c8.svg?invert_in_darkmode&sanitize=true" align=middle width=36.28986404999999pt height=19.1781018pt/> matrix),

<p align="center"><img src="/tex/e462a9d8811d39387c97e322ce5952e3.svg?invert_in_darkmode&sanitize=true" align=middle width=293.33587305pt height=532.17125775pt/></p>

or

<p align="center"><img src="/tex/284b8db7f71dbdc0f2f94b3ecc04cce2.svg?invert_in_darkmode&sanitize=true" align=middle width=351.38692215pt height=465.51294075pt/></p>

In the above, we haven't used any differential technique, because we haven't defined the derivative of vector-by-matrix <img src="/tex/4cd51c073dc2f63ed2a687aabdf9e3c2.svg?invert_in_darkmode&sanitize=true" align=middle width=17.980054949999996pt height=30.648287999999997pt/> which could be a 3D tensor. However, in some cases such as <img src="/tex/fd6a90714b41269dcf4d29fd283b2fc5.svg?invert_in_darkmode&sanitize=true" align=middle width=61.67770949999999pt height=22.55708729999998pt/> (w.r.t. <img src="/tex/380c103b60c66d6420ec8923cdc6e6e8.svg?invert_in_darkmode&sanitize=true" align=middle width=19.80585089999999pt height=22.55708729999998pt/>), the differential technique still works (see [this example](./README.md#y=Wx)).

**E.g. 2**, <img src="/tex/8549adb88bfe36130ebab8cf4798e2e8.svg?invert_in_darkmode&sanitize=true" align=middle width=67.05929834999999pt height=33.20539859999999pt/>, (<img src="/tex/319d907db67f3000780e9b2d1a2816d9.svg?invert_in_darkmode&sanitize=true" align=middle width=14.764759349999988pt height=22.55708729999998pt/> is a <img src="/tex/63b142315f480db0b3ff453d62cc3e7f.svg?invert_in_darkmode&sanitize=true" align=middle width=44.39116769999999pt height=19.1781018pt/> matrix and <img src="/tex/d05b996d2c08252f77613c25205a0f04.svg?invert_in_darkmode&sanitize=true" align=middle width=14.29216634999999pt height=22.55708729999998pt/> is a <img src="/tex/6751b03b5f3d6d66a90def3339c879c8.svg?invert_in_darkmode&sanitize=true" align=middle width=36.28986404999999pt height=19.1781018pt/> matrix),

<p align="center"><img src="/tex/38e2522e1f20b9b702932af1cdd08d64.svg?invert_in_darkmode&sanitize=true" align=middle width=553.9515267pt height=625.9342254pt/></p>

In the above, we haven't used any differential technique, because we haven't defined the derivative of matrix-by-matrix <img src="/tex/67f5bf892d3a85e4355fafecc13c8d5c.svg?invert_in_darkmode&sanitize=true" align=middle width=18.347874599999994pt height=28.92634470000001pt/> which could be a 4D tensor. However, in some cases such as <img src="/tex/20f8bd7d5b5393263f338e8c2a18b2cf.svg?invert_in_darkmode&sanitize=true" align=middle width=65.26671524999999pt height=22.55708729999998pt/>, the differential technique still works (see [this example](./README.md#Y=AX)).