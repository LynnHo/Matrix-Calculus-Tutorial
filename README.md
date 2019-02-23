*read \*.md, do not read \*.tex.md*

<h1> <p align="center"> Matrix Calculus </p> </h1>

In this page we introduce a ***differential*** based method for vector and matrix derivatives (matrix calculus), which ***only needs a few simple rules to derive most matrix derivatives***. This method is useful and well established in mathematics, however few documents clearly or detailedly describe it. Therefore, we make this page aiming at comprehensive introduction of ***matrix calculus via differentials***.

\* *If you want results only, there is an awesome online tool [Matrix Calculus](http://www.matrixcalculus.org/). If you want "how to", let's get started.*

<!-- MarkdownTOC -->

- [0. Notation](#0-notation)
- [1. Matrix Calculus via Differentials](#1-matrix-calculus-via-differentials)
  * [1.1 Differential Identities](#11-differential-identities)
  * [1.2 Deriving Matrix Derivatives](#12-deriving-matrix-derivatives)
    + [1.2.1 Abstract examples: repeat identities 1](#121-abstract-examples-repeat-identities-1)
    + [1.2.2 Actual examples: assisted by identities 2](#122-actual-examples-assisted-by-identities-2)
- [2. Conclusion](#2-conclusion)

<!-- /MarkdownTOC -->


## 0. Notation

- <img src="/tex/332cc365a4987aacce0ead01b8bdcc0b.svg?invert_in_darkmode&sanitize=true" align=middle width=9.39498779999999pt height=14.15524440000002pt/>, <img src="/tex/b0ea07dc5c00127344a1cad40467b8de.svg?invert_in_darkmode&sanitize=true" align=middle width=9.97711604999999pt height=14.611878600000017pt/> and <img src="/tex/d05b996d2c08252f77613c25205a0f04.svg?invert_in_darkmode&sanitize=true" align=middle width=14.29216634999999pt height=22.55708729999998pt/> denote <img src="/tex/06316c77132ca6158472939a99814319.svg?invert_in_darkmode&sanitize=true" align=middle width=45.29889209999998pt height=22.831056599999986pt/>, <img src="/tex/fcc2a3c40b141613d2781dfcfd2690be.svg?invert_in_darkmode&sanitize=true" align=middle width=51.10707194999999pt height=20.87411699999998pt/> and <img src="/tex/7cfa827ff847f043676716fc1761de31.svg?invert_in_darkmode&sanitize=true" align=middle width=79.451658pt height=22.55708729999998pt/> respectively.
- The first half of the alphabet <img src="/tex/5a24655a97800650f252524ec4d77b21.svg?invert_in_darkmode&sanitize=true" align=middle width=79.47848699999999pt height=24.65753399999998pt/> denote constants, and the second half <img src="/tex/068180f9556a78f704df7ad6781b990b.svg?invert_in_darkmode&sanitize=true" align=middle width=80.60117505pt height=24.65753399999998pt/> denote variables.
- <img src="/tex/22acdfc775a9c0010ae19703fdeedeb7.svg?invert_in_darkmode&sanitize=true" align=middle width=24.56618669999999pt height=27.91243950000002pt/> denotes matrix transpose, <img src="/tex/ea1ba186dcad14b51b2f2ed2ff31806d.svg?invert_in_darkmode&sanitize=true" align=middle width=39.90867704999999pt height=24.65753399999998pt/> is the trace, <img src="/tex/9ca9af65e7723587892c4820de37815f.svg?invert_in_darkmode&sanitize=true" align=middle width=23.42461439999999pt height=24.65753399999998pt/> is the determinant, and <img src="/tex/3c7afd910b2b14682613426db256d1ca.svg?invert_in_darkmode&sanitize=true" align=middle width=50.20661909999999pt height=24.65753399999998pt/> is the adjugate matrix.
- <img src="/tex/2cd721f73978bd9ec4aabc24e65b08fd.svg?invert_in_darkmode&sanitize=true" align=middle width=12.785434199999989pt height=19.1781018pt/> is the Kronecker product and <img src="/tex/c0463eeb4772bfde779c20d52901d01b.svg?invert_in_darkmode&sanitize=true" align=middle width=8.219209349999991pt height=14.611911599999981pt/> is the Hadamard product.
- Here we use ***numerator layout***, while the online tool [Matrix Calculus](http://www.matrixcalculus.org/) seems to use ***mixed layout***. Please refer to [Wiki - Matrix Calculus - Layout Conventions](https://en.wikipedia.org/wiki/Matrix_calculus#Layout_conventions) for the detailed layout definitions, and keep in mind that different layouts lead to different results. Below is the numerator layout,

<p align="center"><img src="/tex/1b248f70d5300d3e718064ac71bd7c2e.svg?invert_in_darkmode&sanitize=true" align=middle width=184.37670405pt height=39.452455349999994pt/></p>

<p align="center"><img src="/tex/5f20c4aa8b6cce14bd2fccf73f369229.svg?invert_in_darkmode&sanitize=true" align=middle width=101.1645492pt height=94.143423pt/></p>

<p align="center"><img src="/tex/47bd9b08a8f8ab9758b687d2f3b063cd.svg?invert_in_darkmode&sanitize=true" align=middle width=230.90713965pt height=98.63111444999998pt/></p>

<p align="center"><img src="/tex/43a557c3b375b8ca5dfc60c68f3266f8.svg?invert_in_darkmode&sanitize=true" align=middle width=241.44147225pt height=103.37093415pt/></p>


## 1. Matrix Calculus via Differentials

### 1.1 Differential Identities

- **Identities 1**

<p align="center"><img src="/tex/1367d0cdd0fbd79abf57d0a6d4e5424b.svg?invert_in_darkmode&sanitize=true" align=middle width=410.3851191pt height=235.74932535pt/></p>

- **Identities 2**

<p align="center"><img src="/tex/6959176790cac71173cd72727ebd0ab6.svg?invert_in_darkmode&sanitize=true" align=middle width=629.82298335pt height=294.3619569pt/></p>

- **Identities 1.5 - total differential**. Actually, all identities 1 are the matrix form of total differential in eq. (19).

<p align="center"><img src="/tex/58cbcc2d86dfc0d5e1ec973d164b4f4f.svg?invert_in_darkmode&sanitize=true" align=middle width=495.735801pt height=167.75981309999997pt/></p>

### 1.2 Deriving Matrix Derivatives

To derive a matrix derivative, we ***repeat using the identities 1 (the process is actually a chain rule)*** assisted by identities 2.

#### 1.2.1 Abstract examples: repeat identities 1

**E.g. 1**, <img src="/tex/d6d4dc6b6bbabac486dad7ac3011ac17.svg?invert_in_darkmode&sanitize=true" align=middle width=60.334188749999996pt height=33.20539859999999pt/>.

<p align="center"><img src="/tex/1785e0685f7ee389a54613ef7f82cffd.svg?invert_in_darkmode&sanitize=true" align=middle width=363.51749114999996pt height=80.59222875pt/></p>

finally from eq. (2), we get <img src="/tex/aca022a8d9084c704593d90b61128967.svg?invert_in_darkmode&sanitize=true" align=middle width=74.31442095pt height=30.648287999999997pt/>.

**E.g. 2**, <img src="/tex/3afabb957686c850a9375e82d19dcd8f.svg?invert_in_darkmode&sanitize=true" align=middle width=62.63411055pt height=33.20539859999999pt/>.

<p align="center"><img src="/tex/3316e279dabb3f4cbaee0f558700433e.svg?invert_in_darkmode&sanitize=true" align=middle width=385.11320099999995pt height=124.17602174999999pt/></p>

finally from eq. (3), we get <img src="/tex/330946ab78a470ca64f4e5107987af4b.svg?invert_in_darkmode&sanitize=true" align=middle width=79.69079414999999pt height=30.648287999999997pt/>.

**E.g. 3**, <img src="/tex/fbbdc722022c465f2ae6b48c36598d95.svg?invert_in_darkmode&sanitize=true" align=middle width=63.37669304999999pt height=33.20539859999999pt/>.

<p align="center"><img src="/tex/f840b4416a3f64d656eb04af8c3bbbff.svg?invert_in_darkmode&sanitize=true" align=middle width=386.2404777pt height=114.5869824pt/></p>

finally from eq. (1), we get <img src="/tex/367ed500e49383632c93a4446f39ec80.svg?invert_in_darkmode&sanitize=true" align=middle width=108.3902985pt height=28.92634470000001pt/>.

**E.g. 4**, <img src="/tex/b4d21fc6fdd5d14a267710723a939ba5.svg?invert_in_darkmode&sanitize=true" align=middle width=60.21195674999999pt height=33.20539859999999pt/>.

<p align="center"><img src="/tex/7ef1edf6b0f8989ae7b66a74185a21ef.svg?invert_in_darkmode&sanitize=true" align=middle width=363.5402661pt height=80.59222875pt/></p>

finally from eq. (5), we get <img src="/tex/f8f3b0df92ab2d964857892f8ffec8b0.svg?invert_in_darkmode&sanitize=true" align=middle width=74.31442095pt height=30.648287999999997pt/>.

#### 1.2.2 Actual examples: assisted by identities 2

**E.g. 1**, <img src="/tex/4e82ca6abaed2097dcbead8adf01afec.svg?invert_in_darkmode&sanitize=true" align=middle width=42.555557549999996pt height=37.282175700000025pt/>.

<p align="center"><img src="/tex/9c310a80928421f0554386569eb27c3b.svg?invert_in_darkmode&sanitize=true" align=middle width=439.95767474999997pt height=99.78847065pt/></p>

finally from eq. (2), we get <img src="/tex/c6c1fe4311d8e38885392c2de18807a6.svg?invert_in_darkmode&sanitize=true" align=middle width=94.91611635pt height=37.282175700000025pt/>.

<a name="y=Wx"></a>**E.g. 2**, <img src="/tex/2f241d50ab9d1c15bdbfc64ffdcefbf4.svg?invert_in_darkmode&sanitize=true" align=middle width=70.31119589999999pt height=37.28212289999999pt/>.

<p align="center"><img src="/tex/39d4c566edf7d6adc782e6c16982b883.svg?invert_in_darkmode&sanitize=true" align=middle width=627.40374675pt height=258.7181157pt/></p>

finally from eq. (3), we get <img src="/tex/e5707fda1f7e245c298e383e9f86c6bb.svg?invert_in_darkmode&sanitize=true" align=middle width=195.57101684999998pt height=37.28212289999999pt/>. From line 3 to 4, we use the conclusion of <img src="/tex/d1e757ff485f61fbd67a2c6e31bcf033.svg?invert_in_darkmode&sanitize=true" align=middle width=84.64209435pt height=34.28165400000002pt/>, that is to say, we can derive more complicated  matrix derivatives by properly utilizing the existing ones. From line 6 to 7, we use <img src="/tex/d84c3c399a65b6a8a262aa3315ab4b75.svg?invert_in_darkmode&sanitize=true" align=middle width=66.32411774999998pt height=24.65753399999998pt/> to introduce the <img src="/tex/a4035517c00ae250425f359c6b7eccfb.svg?invert_in_darkmode&sanitize=true" align=middle width=30.182756999999988pt height=24.65753399999998pt/> in order to use eq. (3) later, which is common in scalar-by-matrix derivatives.

**E.g. 3**, <img src="/tex/966fb4dd3b3a91718c1964cff5c791d0.svg?invert_in_darkmode&sanitize=true" align=middle width=49.28919104999999pt height=33.20539859999999pt/>.

<p align="center"><img src="/tex/3f4278ebe0e8315ac8ce2a95ebd102c5.svg?invert_in_darkmode&sanitize=true" align=middle width=449.3987783999999pt height=71.70438164999999pt/></p>

finally from eq. (3), we get <img src="/tex/840804c350d128bab42a8842217b8afb.svg?invert_in_darkmode&sanitize=true" align=middle width=104.29809389999998pt height=33.20539859999999pt/>.

<a name="Y=AX"></a>**E.g. 4**, <img src="/tex/4a3ad3efe4ae7a1b4d75f4b88a821967.svg?invert_in_darkmode&sanitize=true" align=middle width=70.45737435pt height=33.20539859999999pt/>.

<p align="center"><img src="/tex/a7a66e09e9d6d5bdcc6a3e7b9270709f.svg?invert_in_darkmode&sanitize=true" align=middle width=555.8363975999999pt height=65.753424pt/></p>

finally from eq. (3), we get <img src="/tex/a3786564a3359ce0856a2cde2ae2a55f.svg?invert_in_darkmode&sanitize=true" align=middle width=122.08714155000001pt height=33.20539859999999pt/>.

**E.g. 5**, prove <img src="/tex/42f3c1118cca6aa234b8b5726d36587f.svg?invert_in_darkmode&sanitize=true" align=middle width=186.67800359999998pt height=26.76175259999998pt/>.

Since

<p align="center"><img src="/tex/1d94a3056ff8e51a9d5184cc583b69aa.svg?invert_in_darkmode&sanitize=true" align=middle width=79.88556675pt height=17.399144399999997pt/></p>

then

<p align="center"><img src="/tex/a9a3ca06d0cccb54956ca71835c9af3d.svg?invert_in_darkmode&sanitize=true" align=middle width=267.88180485pt height=18.312383099999998pt/></p>

therefore

<p align="center"><img src="/tex/248123e6750f3a3484940afdbf02ca5c.svg?invert_in_darkmode&sanitize=true" align=middle width=192.06611819999998pt height=18.312383099999998pt/></p>

**E.g. 6 - two layer neural network**, <img src="/tex/72e84c4903b48d5de424c69d2dc906b3.svg?invert_in_darkmode&sanitize=true" align=middle width=104.59468799999998pt height=24.65753399999998pt/>, <img src="/tex/2f2322dff5bde89c37bcae4116fe20a8.svg?invert_in_darkmode&sanitize=true" align=middle width=5.2283516999999895pt height=22.831056599999986pt/> is a loss function such as Softmax Cross Entropy and MSE, <img src="/tex/8cda31ed38c6d59d14ebefa440099572.svg?invert_in_darkmode&sanitize=true" align=middle width=9.98290094999999pt height=14.15524440000002pt/> is an element-wise activation function such as Sigmoid and ReLU.

For <img src="/tex/1b029168f72ed78ed025d43ee12a30d5.svg?invert_in_darkmode&sanitize=true" align=middle width=91.66476825pt height=33.20539859999999pt/>,

<p align="center"><img src="/tex/b9d3e768d4e92d59a84014706d278bf4.svg?invert_in_darkmode&sanitize=true" align=middle width=646.51203045pt height=171.41278605pt/></p>

finally from eq. (3), we get <img src="/tex/78a22c94609d25f957a924c8f0c5b7f7.svg?invert_in_darkmode&sanitize=true" align=middle width=311.90916404999996pt height=37.8085191pt/>.

For <img src="/tex/ad8e23aabf92232befd5b06cd73ac69e.svg?invert_in_darkmode&sanitize=true" align=middle width=91.66476825pt height=33.20539859999999pt/>,

<p align="center"><img src="/tex/e56a3fa745579a57417b9d2f6a07ef43.svg?invert_in_darkmode&sanitize=true" align=middle width=718.7442603pt height=349.40093429999996pt/></p>

finally from eq. (3), we get <img src="/tex/e573d73540484e851f8d3ee70e3ace68.svg?invert_in_darkmode&sanitize=true" align=middle width=401.9546586pt height=37.8085191pt/>.

\* *See [examples.md](./examples.md) for more examples.*


## 2. Conclusion
Now, if we fully understand the core mind of the above examples, I believe we can derive most matrix derivatives in [Wiki - Matrix Calculus](https://en.wikipedia.org/wiki/Matrix_calculus) by ourself. Please correct me if there is any mistake, and raise issues to request the detailed steps of computing the matrix derivatives that you are interested in.
