Biotech Notes from DearJohn
=====
<a href="网址">uzi yyds</a>

<font color=red>uzi yyds</font>

|123|234|345|
|:-|:-:|-:|
|abc|bcd|cde|
|abc|bcd|cde|
|abc|bcd|cde|
## 靶向蛋白降解
可以分为溶酶体途径和泛素蛋白酶体途径，前者主要降解膜蛋白，后者主要降解细胞内蛋白
### 泛素蛋白酶体途径
#### 关于泛素
泛素化作为蛋白翻译后修饰（PTM）的方式之一，不仅参与蛋白质的降解，在调节细胞功能方面也发挥着重要作用

泛素为含76个氨基酸、大小约为8.6 kDa的小蛋白质，在真核生物中普遍存在且高度保守。人类基因组中的四个基因编码泛素：UBB，UBC，UBA52和RPS27A。

泛素氨基酸序列：MQIFVKTLTGKTITLEVEPSDTIENVKAKIQDKEGIPPDQQRLIFAGKQLEDGRTLSDYNIQKESTLHLVLRLRGG

泛素具有7个赖氨酸残基（K6，K11，K27，K29，K33，K48，K63）和一个甲硫氨酸残基（M1）。泛素之间主要通过赖氨酸残基和甲硫氨酸残基进行各种连接。由此产生的泛素链产生一定的拓扑结构，可通过对蛋白底物进行修饰并决定底物的功能。

泛素蛋白的结构：

![image](https://user-images.githubusercontent.com/111955215/186657876-63a0363f-7a1a-4719-91d0-b7aba0c145f2.png)

下图为泛素的功能位点:

![image](https://user-images.githubusercontent.com/111955215/186657909-d2b749e7-5195-489e-b4e9-d62a27c52123.png)

泛素降解的机制：

![image](https://user-images.githubusercontent.com/111955215/186657989-5cf6e6b1-a979-4be7-8ab5-646861051d56.png)

## 免疫检查点/immune checkpoint
### PD-1/PD-L1
* **The difference between PD-1 and PD-L1**: 在实际试验中，人们发现达到同样的抑制效果PD-L1的剂量必须非常高，这就导致PD-L1的成本远远高于PD-1。PD1的剂量，大家差不多就是200mg 3周注射一次；PD-L1的剂量，阿斯利康的PDL1 Durvalumab剂量是1500mg 4周一次，故一旦药物价格面临着下行压力，PD-L1商业化价值远远低于PD1。
* PD-1和PD-L1现在存在的问题： 其实除了成本难以下降之外，PD-1的给药方式还是以静脉给药为主，每2~3周一次，虽然现在纳米抗体可以实现皮下注射，但是易用性远不及口服小分子药物。患者依从性：口服＞皮下注射＞静脉注射
## crispr系统
![image](https://user-images.githubusercontent.com/111955215/186565886-532b4a7d-0b7d-44d2-8946-e009b7f0e908.png)

下图右中有俩启动子，可以用**U6启动gDNA，用EF-1a启动Cas9**

![image](https://user-images.githubusercontent.com/111955215/186566329-96b05f44-759e-4963-839e-54199bba6d89.png)

然后再进行下一步的操作

![image](https://user-images.githubusercontent.com/111955215/186566843-aef90271-9f79-41db-b958-778a9598459e.png)

CRISPR/Cas系统可以分为两类：第一类系统的核酸酶由多个亚基组成；第二类系统特别受关注，其核酸酶由单一的蛋白组成，包括基于Cas9、Cas12和Cas13效应蛋白的II、V和VI型。其中最熟悉的 Cas9 蛋白广泛用于基因组编辑等工作，但是CRISPR-Cas9系统也有它的不足之处，即**脱靶效应**。
### 脱靶效应
下图是gRNA的质粒序列

![image](https://user-images.githubusercontent.com/111955215/186557683-6ff9b21b-2369-4094-8fd8-6b7d8834329b.png)

而可能有相当多的相似序列也可能被切掉，如下图

![image](https://user-images.githubusercontent.com/111955215/186557881-0cdfe8f5-a0ff-4563-b302-3ed58b2c4eb5.png)

### cas 13
CRISPR 蛋白家族中的 Cas13 可以靶向RNA 进行基因编辑，其专注靶向RNA的功能补充了靶向DNA的CRISPR-Cas9系统。2016年6月2日，美国麻省理工学院和麻省理工学院-哈佛大学博德研究所的张锋等在《Science》发文，揭示 C2c2 是第一个只靶向RNA而不是DNA的新型CRISPR系统。
不同于靶向DNA的CRISPR相关酶（如Cas9和Cpf1），Cas13a能够在切割它的靶RNA之后保持活性，而且可能表现出不加区别的切割活性，而且在一系列被称作“**附带切割**（collateral cleavage）”的作用当中，继续切割其他的非靶RNA。
![image](https://user-images.githubusercontent.com/111955215/186410590-b32bb595-fa81-468e-bda5-df8ba4d08d7f.png)

### 质粒的构建
<a href="https://www.jianshu.com/p/d97965eb70af">启动子作用功能以及分类介绍_简书</a>

<a href="https://tools.synthego.com/#/">一个很好用的设计网站</a>
#### lentiCRISPRv2系统
![image](https://user-images.githubusercontent.com/111955215/186564662-42edb366-ba0c-4bcc-bcf5-00878ba8ae52.png)

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
