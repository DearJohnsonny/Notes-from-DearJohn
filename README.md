Biotech Notes from DearJohn
=====
<a href="http://eng.chinamil.com.cn/">待到秋来九月八，百花开尽我花杀</a>

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/186898614-eb2f6796-7eca-482b-98a2-c0416ea47912.png" width="1500">
</div>
## 常用的工具
<a href="http://www.unafold.org/mfold/applications/rna-folding-form.php">RNA和DNA的二级结构预测及结果打印</a>

<a href="https://www.jingege.wang/bioinformatics/gene_alias.html">人类基因数据库及其编号</a>

----------
## 甲基化
### DNA甲基化
* **DNA甲基化只能发生在胞嘧啶C上**：即5-mC修饰。其机制为：**胞嘧啶C的5位碳原子**上可以被甲基化修饰，生成5-mC（5-甲基胞嘧啶）。DNA甲基化是在**DNA甲基转移酶**（DNA methyltransferase，DNMTs）的催化下进行的。该反应以**S-腺苷甲硫氨酸（SAM）为甲基供体**将胞嘧啶核苷酸第5位碳原子进行甲基化生成5-mC。

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/186895165-37ffcb12-52f2-444c-a401-e85c0613d604.png" width="480">
</div>

5-mC可以后续被TET家族双加氧酶氧化，依次生成5-hmC、5-fC、5-caC，5-caC进而可以通过TDG等途径被转化为没有修饰的C，从而完成整个甲基化修饰的循环：

![image](https://user-images.githubusercontent.com/111955215/186890558-cc9e258b-958f-43fb-a782-7807c7922e50.png)

* **发生甲基化的“C”在基因组上的分布具有规律**：这些可以被甲基化修饰的胞嘧啶，有一些散落在基因组的各个部分，如外显子、内含子、非编码区等部分；但还有一些C后面会紧跟一个G，加上C、G之间的磷酸基团，我们把它称为“CpG”，这样的CpG往往成簇分布，即在DNA的某个区域能够看到明显较多的CpG，这样的区域叫做CpG岛。

* CpG岛大部分位于基因的启动子区域：据统计，约65%的基因启动子区域附近有CpG岛，这些CpG岛的甲基化成为了调控基因表达的重要方式——**DNA甲基化会抑制下游基因的表达**。DNMT与其它一些蛋白形成蛋白复合物可以识别不同位点的CpG，与去甲基化酶TETs一起，构成了一个重要的基因表达调控体系。如人类女性细胞中含有两条X染色体，其中有一条X染色体是被沉默掉的（X-chromosome inactivation），而DNA甲基化就是X染色体沉默的机制。
#### DNA甲基化与肿瘤
* 机制一：一般来讲，肿瘤的发生总是伴随着整体基因组水平的DNA甲基化的降低，但是，具体到CpG岛的甲基化水平而言，与正常组织相比，肿瘤组织中CpG岛的甲基化水平往往较高。因为CpG岛上升导致被抑制的基因包含不少抑癌基因，（如Rb、BRCA1、CDKN2A、CDH1、VHL等经典抑癌基因），所以GpG岛甲基化水平的上升导致了抑癌基因的失活

![image](https://user-images.githubusercontent.com/111955215/186891090-b6ef9b90-c4f4-42b8-844e-23a88982b566.png)

* 机制二：通过DNA甲基化调控miRNA的表达。当miRNAs的调控区域未甲基化时，miRNAs正常表达，并可能通过降解或翻译抑制使靶基因失活。如果miRNAs以癌基因为靶点，则其作用相当于肿瘤抑制因子。当miRNAs的表达被启动子的甲基化所破坏，靶基因（癌基因）未沉默。正常细胞中由mirRNA沉默的癌基因若可以表达，从而促进肿瘤的发展

![image](https://user-images.githubusercontent.com/111955215/186891151-77696008-1068-4db5-b9c8-20763f93ade3.png)

* 机制三：通过甲基化控制转座子的表达，如果转座子成功表达，会导致产生RNA-DNA杂合双链，从而导致细胞严重坏死，致使肿瘤。

![image](https://user-images.githubusercontent.com/111955215/186891221-1e7e0636-7176-4f9b-b68c-bdc5a1039b8d.png)
#### DNA甲基化和基因沉默
* 	DNA甲基化干扰转录因子对DNA元件的识别与结合；
* 	序列特异性的甲基化DNA结合蛋白与启动子区甲基化CpG岛结合，募集组蛋白去乙酰化酶（HDAC），形成转录抑制复合物，阻止转录因子与启动子区靶序列的结合，从而影响基因的转录；
* 	DNA甲基化通过改变染色质结构抑制基因表达，启动子的高甲基化可导致染色质结构更加紧密进而转录失活。

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/186892133-11721996-a777-470e-972e-b3a87c5df254.png" width="1000">
</div>

![image](https://user-images.githubusercontent.com/111955215/186892195-b09d37a3-157d-4403-8539-b410d3f078e7.png)

## 核酸药物
### 基因沉默药物如miRNA siRNA和shRNA
#### miRNA和siRNA的比较
<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/186809018-39a19a3c-2eae-43ff-9523-faec9612732c.png" width="1200">
</div>

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/186809044-491d59a9-9387-4b32-9b84-8f2f25239eb5.png" width="1200">
</div>

![image](https://user-images.githubusercontent.com/111955215/186809431-2860f56a-a437-4b94-95e5-2d794df12e98.png)

#### miRNA
miRNA一般指micro RNA。MicroRNA (miRNA) 是一类由内源基因编码的长度约为19-24nt的非编码单链RNA分子，它们在动植物中参与转录后基因表达调控。miRNA通常位于基因间（intergenic）或位于内含子（intronic)区域，因此普遍认为它并作为编码其他类型基因的一部分而被转录，这些小分子RNA通过碱基配对与靶mRNA序列的3'UTR区或编码区结合，剪切靶基因的转录产物或者抑制转录产物的翻译，从而调控基因的表达。

![image](https://user-images.githubusercontent.com/111955215/186809104-4e6b0834-5fa8-4161-9a09-b0fb8ba2174a.png)
#### shRNA
从结构上看shRNA和miRNA更相似，事实上shRNA在功能上与siRNA更接近。shRNA在细胞内被Dicer酶切割后形成siRNA，通过siRNA途径行使干扰功能，而miRNA则是通过另一条不同的途径调控目标基因。
shRNA实际上是通过载体构建在体内获取siRNA的一种方式，两者结构本质上是相同的，但在功能上有所差异。
shRNA是可以克隆至表达载体并表达双链siRNA的RNA分子，包括两个短反向重复序列，中间由一茎环序列分隔，形成发夹结构，由polⅢ启动子控制。相对于siRNA，shRNA在细胞核中合成，进一步加工并运输到细胞质中，然后进入RISC发挥活性。miRNA的合成与成熟研究为shRNA的合成，特别是基于miR-30的shRNA的合成提供了基础。![image](https://user-images.githubusercontent.com/111955215/186809372-15fc2a60-e036-498d-ad68-a621ed7c9373.png)

![image](https://user-images.githubusercontent.com/111955215/186809306-52a2795f-dcab-4c7e-b98a-04efbba9b2a0.png)
### ASO反义核苷酸药物
反义寡核苷酸(ASOs)被定义为化学合成的寡核苷酸，通常长度为12-30个核苷酸，目的是通过Watson-crick碱基配对规则与RNA结合。
![image](https://user-images.githubusercontent.com/111955215/186809553-4536089e-8f7c-4394-b43c-3b0f0409740c.png)

* 占位机制：通过与细胞核内的pre-mRNA互补，导致poly-A的尾不能正常形成或剪接成熟不能进行；通过与细胞核外的成熟mRNA结合，导致其翻译不能正常进行

![image](https://user-images.githubusercontent.com/111955215/186810198-feeab0e5-b548-4c7f-8d9b-efdec47122e0.png)

* RNA降解机制：通过招募RNase H1或Argonaute 2(Ago 2)降解RNA
 
![image](https://user-images.githubusercontent.com/111955215/186810609-721a4f4b-a844-4c1e-9fa2-e89e4e219783.png)
* 抵抗miRNA的降解：通过与miRNA形成base pair抵抗其降解作用，此机制为上调

## 细胞衰老
### 细胞衰老的标志
* **衰老相关-β-半乳糖苷酶的表达**(senescence-associated-β-galactosidase，SA-β-gal)：一种溶酶体酶。该标记物在大多数衰老细胞中可通过组织化学染色检测到，而在未衰老的，静息的或永生的和转化的细胞中一般不存在
* **形态异常增大、扁平，胞质核比不成比例地增加**。虽然这种体积庞大的细胞质最初被描述为**伴随**细胞衰老形成的特征，但最近的一项研究表明，细胞大小的增加可能在衰老相关的生长停滞中起着重要作用。
* **缺乏DNA复制**
### 衰老与自噬
功能障碍的细胞器，如线粒体和溶酶体，通常通过激活细胞内名为“自噬”的降解系统而被降解。然而，到底自噬是一个促进衰老的诱发因素，还是一种在衰老过程中开始起作用的负调控机制（抑制衰老）仍然值得研究。
有研究表明，自噬是由衰老触发的，以应对有毒大分子积累导致的负荷增加，自噬的药理靶向性导致衰老细胞被消除。然而，自噬也被认为通过促进受损细胞器和其他细胞成分的降解来抑制衰老。
### 衰老与DNA损伤
核DNA损伤会促使细胞衰老，主要表现为可激活DNA损伤应答（DNA damage response，DDR）的DNA双链断裂（DNA double-strand breaks，DSBs）的积累。
DDR发挥检查点功能来阻断细胞周期，如果DNA损伤持续存在，它会导致DDR信号的延长和以细胞衰老为形式的持久性增殖阻滞。抑制DDR信号激酶（ATM、ATR、CHK1和CHK2）使衰老细胞重新进入细胞周期。
在DDR级联效应的后期，肿瘤抑制物p53被激活（p53是ATM及其旁系同源物ATR的靶点）并刺激细胞周期素依赖性激酶抑制剂p21的表达（p21是衰老相关细胞周期阻滞的重要介质）。p16是CDK4和CDK6的抑制剂，也是几种衰老类型的关键酶；p21在衰老早期被激活，p16在衰老后期被激活，可能是为了维持衰老表型。
![image](https://user-images.githubusercontent.com/111955215/186671723-e50a3aa2-cebe-41db-9c60-048b92224de9.png)
### 衰老与端粒缩短
由于标准的DNA复制程序无法完全复制染色体DNA末端，在没有端粒维持机制的情况下，如端粒酶的表达或端粒之间的重组，端粒随着每一轮DNA复制而缩短。在一定长度以下，端粒封闭因子或保护结构的丢失使端粒非常短，类似于单端DSBs，从而触发与DNA DSBs触发的DDR非常相似的DDR

<a href="https://www.jingege.wang/2022/02/26/nature/">其他的衰老相关的问题可以看这个汉化版的Nature综述</a>
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
