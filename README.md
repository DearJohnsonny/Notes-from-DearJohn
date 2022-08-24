# To start with
<a href="网址">名字</a>
## crispr系统
### 质粒的构建
<a href="https://www.jianshu.com/p/d97965eb70af">启动子作用功能以及分类介绍_简书</a>
#### lentiCRISPRv2
BsmBI site的开头是CACC,结尾是CAAA。设计oligo的时候要确保在开头的基础上加G，以确保稳定性。
所以设计Oligo的时候是：
Forward：5' - CACCG - 20bp - 3'
Reverse：5'- AAAC -20bp（Copy bottom strand 5'->3） - C - 3' (注意后面还跟一个C！！！)
Oligo粘合之后，应该长成下图这样：

![image](https://user-images.githubusercontent.com/111955215/186406530-b17607c1-c78f-46f4-bcbf-36ccb22dd857.png)

<a href="https://www.jianshu.com/p/6de326895f5b">SgRNA and lentiCRISPRv2_简书</a>

<a href="https://www.jingege.wang/2020/05/29/crispr-cas9-sgrna%e8%ae%be%e8%ae%a1%e5%92%8c%e8%bd%bd%e4%bd%93%e6%9e%84%e5%bb%ba/">CRISPR-Cas9 sgRNA设计和载体构建</a>

<a href="https://zhuanlan.zhihu.com/p/34561875">CRISPR sgRNA Oligo设计_知乎</a>
## Phage Display
噬菌体展示技术有多种分类标准。根据噬菌体的不同，可以分为M13、T7、T4、λ等多种体系；根据载体的不同，可以分为噬菌体载体（True Phage）和噬菌粒载体（Phagemid）；根据文库的不同，可以分为随机肽库、cDNA文库、抗体文库、蛋白质文库等。
抗体库的筛选是指从抗体库中筛选出针对某一抗原的特异性抗体，是获得高亲和力抗体过程中的关键环节。单克隆抗体性质存在千差万别，需根据不同的单抗制定严格的筛选条件，一般分为经典筛选法和新型筛选法。
### 经典筛选法
主要为固相筛选法和液相筛选法，用于抗原性质明确的抗体筛选。固相筛选法通过包被在酶标板或其他固相介质上的抗原富集高亲和性的噬菌体；液相筛选法(如下图)是将生物素化的抗原包被在与亲和素偶联的磁珠或琼脂糖上，进行抗原特异性结合的方法。通过多次筛选，抗原得到高亲和力的噬菌体。
![image](https://user-images.githubusercontent.com/111955215/186395522-6735bf29-58da-4889-9b65-70f5731ee7f6.png)
### 新型筛选法
当抗原无法纯化或性质不明时，就需要开发新的筛选方法，用于抗体库的建立。目前比较成熟的有细胞筛选法、组织切片或体内筛选法、选择感染筛选法、蛋白质芯片筛选法等。
细胞筛选法可以维持抗原和抗体的天然构象，多用于肿瘤细胞抗体筛选，还适用于细胞表面受体及抗原鉴定。但由于细胞膜表明成分复杂，会增加非特异性结合，而多次筛选又容易丢失特异性结合的抗体，因此限制了此方法的应用，并且在此方法基础上开发了扣除筛选、竞争筛选、内化筛选等方法。
