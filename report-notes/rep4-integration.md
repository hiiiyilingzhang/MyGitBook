# 😣 Rep4 integration

### DoubletFinder--Singleron doublet rate

![](../.gitbook/assets/image.png)

p1-blood: 0.037\*8916=329

p1-ERM: 0.01\*3097=30

p2-blood: 0.04\*9595=382

p2-ERM: 589

0630-blood: 0.03\*8603=258

0630-ERM: 0.0075\*2520=18

0609-blood: 0.048\*11865=569

0609-ERM: 0.002\*1255=2

**Totle: 1796**

### 不要靠近kBET 会变得不幸

基于奇异值降解的基础上进行降维

算法的主要假设是 如果临近样本的子集标签分布与完整数据集的分布相同，则表明该重复实验能够很好的混合，相反，在存在批次效应下，生物学重复将会在整个数据集中产生批次标签的倾斜分布。KBET 通过采用卡方分布检测固定大小的随机邻域从而确定它们是否很好的被混合了。然后是得到一个二进制的结果用来计算后续的拒绝率，这表明，拒绝率越低样本混合的越好。

![134bil](<../.gitbook/assets/image (1).png>)

![](../.gitbook/assets/image-20211013223446241.png)

### LISI

[https://github.com/immunogenomics/LISI](https://github.com/immunogenomics/LISI)

> Learn more about how we use LISI to measure single cell integration methods in the Harmony paper: Korsunsky, I. et al. [Fast, sensitive and accurate integration of single-cell data with Harmony.](https://www.nature.com/articles/s41592-019-0619-0) Nat. Methods (2019)

### Harmony给爷爬

![](<../.gitbook/assets/image-20211014163420710 (1).png>)

[https://github.com/immunogenomics/harmony/pull/134](https://github.com/immunogenomics/harmony/pull/134)

要先call `library(Rcpp)`和`library(rlang)`

新版已经fix

![](../.gitbook/assets/image-20211014163933014.png)

### X11 connection error

![](../.gitbook/assets/image-20211015164921588.png)

![](../.gitbook/assets/image-20211015164934206.png)

stackexchange上的法子都不管用，需要root装依赖？无所谓了随便吧，反正rmd能输出就行

### Comparison between Harmony & Seurat integration

* harmony

![](<../.gitbook/assets/image-20211015183214339 (1).png>)

![](../.gitbook/assets/image-20211015183355315.png)

* Seurat

![](<../.gitbook/assets/image-20211015203241348 (1).png>)

![](<../.gitbook/assets/image-20211015203312754 (1).png>)

* Seurat is better than harmony in this situation

## scclusteval

**Evaluating single-cell cluster stability using the Jaccard similarity index**

[https://academic.oup.com/bioinformatics/article/37/15/2212/5962080](https://academic.oup.com/bioinformatics/article/37/15/2212/5962080)

[https://github.com/crazyhottommy/scclusteval](https://github.com/crazyhottommy/scclusteval)

do it later

### 哈？？？？？啥玩意儿

![](../.gitbook/assets/image-20211017114521403.png)

### 注释用哪个assays

![](<../.gitbook/assets/image-20211018080250598 (1).png>)

我用的SCT





### Rmd is here

{% file src="../.gitbook/assets/Report4_integration.Rmd" %}

\
