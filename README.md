Notes from DearJohn
=====
<a href="https://dearjohnsonny.github.io/Notes from DearJohn-2/">Notes from DearJohn-2</a>

<a href="https://dearjohnsonny.github.io/Notes3-Statistics/">Notes3-Statistics</a>

<a href="https://dearjohnsonny.github.io/Notes4-Linear-Algebra/">Notes4-Linear-Algebra</a>

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/186898614-eb2f6796-7eca-482b-98a2-c0416ea47912.png" width="1500">
</div>


## 常用的工具
<a href="http://www.unafold.org/mfold/applications/rna-folding-form.php">RNA和DNA的二级结构预测及结果打印</a>

<a href="https://www.jingege.wang/bioinformatics/gene_alias.html">人类基因数据库及其编号</a>

## 干扰素通路
### TLR受体
在人体免疫细胞表面有一类识别病毒及细菌等病原体的受体（PRR），识别内容是病原微生物的核酸或是细胞膜成分等，这是细胞抵御病原体入侵的第一道防线。研究发现，这类受体（PRR）主要是Toll 样受体(TLRs)，目前已发现11个 TLR 家族成员，其中 TLR1、TLR2、TLR4、TLR5、TLR6 和 TLR11 位于细胞表面，而 TLR3、TLR7、TLR8 和 TLR9 位于内体/溶酶体部分。大家都比较清楚，病毒的主要结构是遗传物质DNA或者RNA及包膜蛋白，TLR3 and TLR7/8能特异性识别病毒RNA，TLR9识别病毒的CpG-DNA。
![image](https://user-images.githubusercontent.com/111955215/187031388-43e5de37-038a-4a19-b975-06f9cf679f13.png)

### 关键的转录因子NF-kB和IRF3
在STING发现以前，大量的研究已经表明两类重要的转录因子（transcription factors），一个是NF-kB，另一个是IRF3，这两个转录因子都能在病毒入侵时诱导一系列基因表达谱发生改变以产生病毒抵抗。其中，NF-KB主要是诱导促炎性细胞因子表达，而IRF3主 要是诱导I型干扰素表达。

![image](https://user-images.githubusercontent.com/111955215/187031426-6db043db-58a2-4d0d-bf66-5cdb2742368d.png)

后来发现：STING是TBK1/IRF3的上游，STING定位于内质网膜，并且激活NF-κB和IRF3下游信号通路，在抗病毒免疫中发挥关键作用

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/187031503-d0a0d1fe-0b55-4cf0-a5cb-bfc60198601e.png" width="300">
</div>

### dsDNA和病毒的干扰素通路
![image](https://user-images.githubusercontent.com/111955215/187031446-3ffe9375-bdbb-438f-80bc-93f36683ac5a.png)

### 干扰素作用机制
三种干扰素的受体激活机制及受体-配体复合物组成：
![image](https://user-images.githubusercontent.com/111955215/187031492-5cce00fa-e0d4-4a14-b9aa-9f00a0fcb8a4.png)

### 干扰素作用途径
![image](https://user-images.githubusercontent.com/111955215/187031522-216d846f-cc64-4f6d-b897-486f6df023b0.png)

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/187031359-4b8874c3-d70d-4a1c-87b4-ad8469f6c41c.png" width="1500">
</div>

## 外源性DNA抗性机制
哺乳动物体内主要有三种针对外来DNA的免疫反应：TLR9（Toll-like receptor 9）引发、AIM2（absent in melanoma 2）和cyclic GMP–AMP synthase (cGAS)途径。
### TLR9通路
TLR9位于内体膜，主要感应CpG岛未甲基化的DNA，然后激活转录因子NF-κB（nuclear factor-κB），IRF7（interferon regulatory factor 7）从而导致编码炎症细胞因子和干扰素的基因高表达。

![image](https://user-images.githubusercontent.com/111955215/187030875-8f329103-0dce-4008-b7c6-c54f537ecb13.png)
### AIM2通路
AIM2和细胞质的双链DNA结合，导致AIM2炎症小体的形成，激活caspase1和IL-1β和IL-18的释放，最后导致细胞死亡。
### cGAS-STING通路
cyclic GMP–AMP synthase的激活导致GMP和AMP成环，形成cyclic GMP–AMP，这个第二信使会和STING蛋白结合，调控其活性，导致TBK1（TANK-binding kinase 1） ，TBK1会导致STING和 IRF3的磷酸化从而激活，最后使得一型干扰素高表达。STING的激活同时会导致NF-κB的激活，NF-κB激活既会促进一型干扰素的表达，也会促进IL-6和TNF的产生。

![image](https://user-images.githubusercontent.com/111955215/187030932-e0f499eb-2c64-4e0e-bbe2-e1d4a2219093.png)

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/187030764-5aca726d-1787-4fe8-bcfd-289b144ab582.jpg" width="1500">
</div>

## DNA纳米技术
### DNA walker
下面这个是2004年的原始文献，系统由4个部分组成：walker (W), track (T), attachment fuel strands (A), and detachment fuel strands(D)。D的作用是将两个已经形成双链的W解掉前一个双链。

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/187811782-7082eaf5-2574-44c5-bc73-9b9f0463944c.png" width="700">
</div>

DNA walker的动力学：

![image](https://user-images.githubusercontent.com/111955215/187817008-36724bab-ad4e-4303-9884-70ccffe386ac.png)

现在的DNA walker有以下几种类型

![image](https://user-images.githubusercontent.com/111955215/187816591-7a98e379-2701-409a-aba6-989fce4163a8.png)

还可以用来解除二级结构——catalytic hairpin assembly (CHA)：

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/187821060-6dc24a9d-111f-45a5-a49e-bca622cea927.png" width="800">
</div>

主要是通过荧光来进行检测，与beacon或者probe之类的结合：

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/187821054-aad323a9-501b-4c1e-a384-1b047a7b2fbf.png" width="800">
</div>

下图也是：

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/187821950-296e107a-db9c-4102-95b2-90e8c4c21571.png" width="800">
</div>

下图也是：

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/187822546-3c477827-eed2-4344-bb11-b1194f97efaf.png" width="800">
</div>

#### 一些DNA walker的奇思妙想
下图工作是为了检测溶酶体，通过与溶酶体的结合制备Y-WS并进一步制造出金纳米颗粒的toehold，并与Tt结合，从而释放出带有荧光的片段

![image](https://user-images.githubusercontent.com/111955215/187813480-9b579df7-7447-4f2f-8f63-9b592022a38f.png)

### 应用
#### 组织engineering
![image](https://user-images.githubusercontent.com/111955215/187016831-173aa1f1-a02b-4e41-a942-5b1d2f8fc856.png)
#### 辅助核酸递送
如果直接递送核酸（如质粒、ssDNA和ssRNA），可能会被溶酶体降解；但是如果搭配一些纳米材料则可以减少上述情况的发生

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/187016994-48d5eeb1-a73a-4a03-83ca-d0df0f28291b.png" width="1500">
</div>

#### 搭载药物同时外嵌靶头
外侧嵌合一个可以靶向肿瘤细胞的靶头，纳米结构内部包含杀伤肿瘤的药物，起一个递送药物的作用，减少脱靶效应

![image](https://user-images.githubusercontent.com/111955215/187017170-e21f6284-319d-4cd2-af25-ab87915f3375.png)

#### 构建免疫反应触发体
CpG不是CpG岛而是一小段核酸：The vertebrate immune system has the ability to recognize thepresence  of  bacterial  DNA  on  the  basis  of  recognition of so-called CpG   motifs, unmethylated cytidine-guanosinedinucleotides within a specific pattern of flanking bases.

CpG-DNA是一类以CpG二核苷酸为核心的未甲基化的特殊DNA序列，可以激活免疫活性细胞产生多种细胞因子。
研究发现，细菌DNA具有20折叠的高频率未甲基化的CG二核苷酸，可引起急性炎症反应，通过对细菌DNA和脊椎动物DNA的对比发现，CpG-DNA引起的细胞激活经由Toll/IL-1R信号通路发生。TLR9是CpG-DNA受体的一个重要组成，直接和CpG-DNA结合。合成的Oligo脱氧核苷（ODN）包含特有的CpG-DNA以达到模仿细菌DNA的免疫刺激效果，还能影响免疫耐受和自身免疫性疾病。CpG-DNA应用广泛，在肿瘤治疗、提高机体免疫力和抗寄生虫等方面都有应用。

![image](https://user-images.githubusercontent.com/111955215/187031271-a3593cac-7314-4cf9-9d98-a5b0c0700287.png)

![image](https://user-images.githubusercontent.com/111955215/187017176-d890eb39-295d-47a2-8654-f15bbed96fd9.png)

#### 细胞内诊断和成像的作用
进入细胞之后通过特定的结合（如pepper这种aptamer的结合之后产生荧光），帮助诊断

![image](https://user-images.githubusercontent.com/111955215/187017279-f4440167-2194-4557-b93f-3d0edef20804.png)

#### 病原体的检测
如果病原体可以结合，就会将cDNA从珠子上顶替下来，然后对在溶液中的cDNA进行扩增，并切去引物，新得到的ssDNA可以组装成理想的纳米结构，并可以搭载荧光基团从而被检测到

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/187017443-58ff1729-bc33-4dfd-b991-aa7f7498eeca.png" width="800">
</div>

<a href="https://www.sohu.com/a/482872459_121124715">其他纳米结构DNA辅助病原体检测的方法都在这</a>

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/187016796-b39a386b-25ca-4ad7-bc21-8d6b9aaf92b4.png" width="1500">
</div>

## 关于核酸药物的递送
### AVV
腺相关病毒（Adreno-Associated Virus, AAV）是微小病毒科（Parvoviridae）家族的成员之一。这一家族成员是一类微小、无被膜及具有二十面体结构的病毒。病毒颗粒的直径在20～26nm之间，含有大小在4.76kb之间的线状单链DNA基因组。它的复制和增殖依赖于辅助病毒的存在。
它由直径约26nm的二十面体蛋白质衣壳和~4.7 kb的单链DNA基因组组成。衣壳包含三种类型的亚基VP1、VP2和VP3，总共60种拷贝，比例为1:1:10(VP1:VP2:VP3)。基因组的两端是两个T形反向末端重复序列(ITR)，其末端主要用作病毒复制起点和包装信号。rep基因编码病毒复制所需的四种蛋白质；它们以其分子量命名：Rep78、Rep68、Rep52和Rep40。cap基因通过来自不同起始密码子的可变剪接和翻译编码三个衣壳亚基。此外，编码组装活化蛋白(AAP)的第三个基因在不同阅读框中的cap编码序列内编码，并且已显示出促进病毒粒子组装。

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/186907142-fc119948-ebc1-46cb-a628-7b30c7726cb7.png" width="600">
</div>

关于重组腺病毒载体递送药物：

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/187110462-5f60e3f2-6033-49c7-b788-0b41a540ec50.png" width="900">
</div>

#### AAV的作用机制
AAV会和糖基化的细胞表面受体结合，并被吞入细胞内，形成初级内体，此后再形成次级内体。次级内体的AAV会被转运进入细胞核，并释放出DNA。

目前主要的重组的rAAV有两类：一类（ single-stranded AAV ，ssAAV）是未形成互补链的单正链或单负链，需要先利用宿主的DNA聚合酶形成互补链，或者与同时转入细胞核的互补链退火互补；另一类（self-complementary AAV ，scAAV）在设计之时已经为互补单链。形成互补链之后， rAAV的基因组中的inverted terminal repeats (ITRs)会促成已经形成互补链的DNA分子的重排，从而形成环状的核内DNA分子（episome）。该环状DNA分子偶尔会插入到宿主的基因组中，多数时候不会起作用，可以长期随细胞保留（一般时间长达5个月）。通常情况下 AAV 不能独立复制，只有在辅助病毒（如腺病毒，单纯疱疹病毒，痘苗病毒）存在时，才能进行复制

AAV 包装过程中，包装质粒负责编码目的基因以及两个末端反向重复序列（ITR，对于病毒的复制和包装具有决定性作用），辅助质粒包含 AAV 包装所需的cap（编码病毒衣壳蛋白）和rep（参与病毒的复制）基因，以及腺病毒 Helper 质粒。三种质粒共同转染 293T 细胞后，AAV 病毒开始复制和包装。

![image](https://user-images.githubusercontent.com/111955215/186907292-53dd763b-3068-452e-945e-c6b2cb13606e.png)
#### AAV的劣势
* AAV有一定概率会产生免疫反应。如果曾经感染过某些病毒或者此前接受过AAV治疗，再注射会被免疫系统识别，AAV在没有递送到目标之前就被清除掉了
* AAV基因片段会插入到细胞基因控制生长的区域，可能会导致肿瘤发生。此前大家都认为AAV游离在染色体外，不会整合到基因组，但是，近些年的一些研究发现，AAV有较低概率可以整合至基因组，且这种整合存在随机性，如果它整合至关键区域，就有可能产生致癌风险————不过，AAV基因组可以整合到人细胞中称为AAVS1的基因组基因座中以建立潜伏期。这种现象部分是由于AAVS1中发现的序列相似性以及ITR和Rep活性。如下所述，因为rAAV缺乏rep基因，所以rAAV基因组整合大大减少
* AAV容量有限，最大可以容纳大概4.7kb，而治疗一些疾病所需的DNA序列和基因编辑工具的嵌合体都超过了这个容量限制，比如CRISPR/CAS基因编辑工具，CAS和gRNA就必须被分别封装在两个AAV衣壳里，再递送到同一个细胞里拼装，增加了复杂性
* 虽然目前AAV载体在眼科、肝脏等疾病方面实现了拉长给药间隔时间的目标，但是由于不整合到基因组，AAV无法随细胞进行复制从而被稀释，仍然存在需要重复给药的问题，尤其是在第一针注射AAV后，若产生免疫原性，将无法为病人提供第二次治疗，这将导致AAV很难做到对某一种疾病的终身治愈

### LNP
递送常规药物的LNP：

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/187108017-aa72a7df-61d7-4d41-9450-e45f70045ed4.png" width="700">
</div>

递送核酸药物的LNP：需要在内部添加一些带有正电的脂质以稳定负电性的核酸
<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/187108491-5a72c008-71c2-410c-a094-f6d38447627c.png" width="700">
</div>

#### 递送mRNA的优势
首先明确递送mRNA的挑战：
* mRNA带负电，而细胞膜也带负电，mRNA会因为静电排斥难以进入细胞
* mRNA分子是单链，本身极其脆弱，体内的多种酶都能将它迅速降解

载mRNA的脂质纳米粒（Lipid nanoparticle,LNP）除了含有带负电荷的mRNA外，另有**四种成分**：可电离的阳离子磷脂（ionizable lipids），中性辅助磷脂，胆固醇，聚乙二醇修饰的磷脂（PEGylated lipid）。
中性辅助磷脂一般为饱和磷脂，可提高阳离子脂质体的相变温度，支持层状脂质双层结构的形成并稳定其结构排列；胆固醇有较强的膜融合性，促进mRNA胞内摄入和胞质进入；PEG化磷脂位于脂质纳米粒表面，改善其亲水性，避免被免疫系统快速清除，防止颗粒聚集，增加稳定性。最关键的辅料是可电离阳离子磷脂，它是mRNA递送和转染效率的决定性因素。

![image](https://user-images.githubusercontent.com/111955215/186909584-c5d1fdc7-9ad2-4493-8df4-08e33b47f2eb.png)

#### mRNA/LNP作用机制
入胞前，阳离子脂质可实现与带负电荷的mRNA分子静电络合，形成复合体，提高mRNA分子的稳定性。mRNA/LNP到达细胞膜时，阳离子磷脂与带负电荷的细胞膜触发膜融合，细胞膜去稳定化，促进mRNA分子的递送。内化进入细胞后，随着含有多种水解酶的溶酶体分解外源和外源大分子，pH值降低形成偏酸环境，使可离子化的脂质质子化，LNP的双层结构遭受破坏，释放mRNA，按照“中心法则”与负责生产蛋白的核糖体结合，翻译成病毒蛋白，即抗体，中和病毒。

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/186910701-a02fce70-943d-4d4b-ac20-da44e4317735.png" width="600">
</div>

### 外泌体
外泌体（exosome）是由细胞内多泡体(multivesicular body，MVB) 与细胞膜融合后，释放到细胞外基质中的膜性囊泡。几乎所有类型的细胞，都可以产生并释放外泌体。它是一种直径为30-100nm的纳米级脂质包裹体结构，内部包裹了蛋白、mRNA和microRNA等物质。外泌体天然存在于体液中，包括血液、唾液、尿液和母乳，被分泌出的外泌体会进入血液、唾液、尿液、及乳汁等体液中，通过循环系统到达其他细胞与组织，产生远程调控作用。

![image](https://user-images.githubusercontent.com/111955215/186913676-917a2b00-59d7-4f36-95ae-bfc219c738a4.png)

* Structure and composition of exosomes:

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/187108880-beea1d08-cb8b-4d57-8dfb-b38ca32f181c.png" width="700">
</div>

* **Surface engineering** of exosomes via genetic/biological manipulation or chemical modification:

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/187108939-b8a0ed7d-d221-4db6-bd1a-6caf7b2ad4e0.png" width="700">
</div>

#### 外泌体的应用
将蛋白质转入细胞：

![image](https://user-images.githubusercontent.com/111955215/186913785-f8cd0bd0-c830-4f4d-992e-92d17f658ded.png)

将RNA转入细胞：

![image](https://user-images.githubusercontent.com/111955215/186913818-7844a909-9db7-4efb-ad87-a08691754a25.png)

#### 外泌体的优势
* 通过工程化修饰，可靶向到特定的组织和器官，解决传统递送系统无法解决的问题；
* 无免疫原性，包裹的核酸药物不易降解，降低药物全身暴露毒性；
* 可跨越血脑屏障，实现颅内药物递送。

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/186913346-99cd16d5-4270-4c23-869c-c50f6ede1716.png" width="1500">
</div>

## Z-DNA
<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/186901257-de1eb4d5-68ac-4e3c-b686-37e942c0420e.png" width="600">
</div>

### 区别Z-DNA和Spiegelmers
* Z-DNA都是D型核苷酸组成的，而Spiegelmers的单体就是L型核苷酸
* Z-DNA是天然存在于人体及细菌界中的，而Spiegelmers是人工合成的
* 两者都能通过与canonical的核酸差异而产生一定的原有的核酸酶抗性

### Z-DNA与微生物的胞膜形成
Z-DNA是具有未成熟生物膜的eDNA的主要结构形式，B-DNA是形成Z-DNA的eDNA库。抗核酸酶的Z-DNA，对维持细菌生物膜的稳定性至关重要；为了将Z-DNA转化为B-DNA，作者使用了DNA插入剂氯喹，它可以防止Z-DNA的形成；相反：多价阳离子或高离子强度（CeCl3，氯化铈）也能促进B-DNA向Z-DNA转化

###  Z-DNA与细胞凋亡
![image](https://user-images.githubusercontent.com/111955215/187074049-edf02329-a96f-4623-9d5a-ff2f34dc288b.png)

#### Z-DNA结合蛋白与中暑的关系
在heatstress的环境下培养细胞发现会促使细胞的**RIPK3**和**MLKL**的磷酸化；hotstress的环境下培养还会造成凝血酶的增多、血小板的增多、纤维蛋白的沉积还有血管微循环的闭塞，而敲除RIPK3基因后上述心血管不适减弱。实验证明ZBP-1是RIPK3的上游蛋白，可以激活RIPK3。
病原体入侵——heatstress—— HSF1（heat shock transcription factor1 ）——ZBP-1——RIK3——MLKL——细胞坏死

### 关于ADAR
ADAR最初被发现是由于其具有将A→I的功能。

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/194537274-c8188f9c-70b1-4ac8-873f-e4755d2e1485.png" width="1500">
</div>

(A) ADAR 家族由三个成员组成。两种 ADAR1 亚型，一个长 p150 (1226aa) 和一个短 p110 (931aa)、ADAR2 (701aa) 和无催化活性的 ADAR3 (739aa)。 ADAR1p150 和 ADAR1p110 中存在的 Z-DNA 结合域以绿色表示。双链 RNA 结合域 (dsRBD) 和脱氨酶域 (editase)，分别以蓝色和红色表示，存在于所有三个 ADAR 中。 ADAR1p150 含有一个核输出信号（NES；橙色），说明其细胞质定位，而所有成员都带有一个以黄色描绘的核定位信号 (NLS)。 R 域以紫色表示，使 ADAR3 能够与单链 RNA (ssRNA) 结合。 (B) ADAR 与双链 RNA (dsRNA) 结合并将腺苷残基脱氨基，将其转化为肌苷。肌苷不再与尿嘧啶配对，因此它的存在将 dsRNA 展开为 ssRNA。肌苷与鸟苷具有相同的化学性质，因此被细胞机器进一步识别为鸟苷。

ADAR1基因会转录出两个亚型：ADAR1 p150和ADAR1 p110。其中ADAR1 p110没有Zα结构域，这是ADAR1和Z-DNA/RNA结合的关键。

研究表明，人ZαADAR1 对 Z-DNA 具有高度的亲和性，而ZβADAR1对Z-DNA的亲和性很弱甚至不能与其结合。Zα结构域是和已经形成的Z-DNA结合，而不是通过诱导产生Z-DNA并与之结合。Zβ的功能尚且不太明确；Zα结构域除了特异性识别和结合 Z-DNA 外，也能与 Z-RNA 结合，结合机制基本一样。

#### Role of ADAR1-induced RNA editing in the suppression of innate (auto)immune response
病毒感染后，通过对dsRNA的响应（MDA5蛋白识别dsRNA → MAVS蛋白被MDA5激活 → MAVS激活ISG），ISG转录增加；Interferon-stimulated genes (ISG)转录后，ADAR1 p150和一型干扰素被转录。
而dsRNA的来源主要为转座子（人的基因组序列中一半以上为转座子产生的序列）。外源性基因（病毒基因）通过转座子随机整合到宿主细胞基因组内后（在进化的过程中多种病毒的dsRNA序列被转入人体，成为现在人基因组内高度保守的序列），利用宿主细胞进行转录时，常产生一些dsRNA。Alu SINE的序列占基因组中约10%，而Alu被ADAR编辑（即I→G，导致突变）。

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/194537623-70b96e8d-ae79-4e40-af63-e23fafc7c1d8.png" width="1500">
</div>
(A) dsRNA 被双链 RNA 传感器（dsRNA 传感器）识别，即 MDA5 和 RIG-I。 激活后，RIG-I 和 MDA5 受体都通过线粒体抗病毒信号转导蛋白接头发出信号，进而导致 NF-κB 和 IRF3/7 的激活以及随后 I型IFN和ISG的上调，从而引发先天免疫反应。(B) ADAR1 编辑位于细胞质中的长 dsRNA，抑制 MDA5 或 RIG-1 的下游识别。 该事件导致先天免疫反应的整体抑制。

#### Main molecular consequences of ADAR-induced RNA editing
<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/194538051-64930e83-cb2f-4c8c-8487-3b49a9d8c8e5.png" width="1500">
</div>

ADAR1 或 ADAR2 (ADAR1/2) 诱导的编码 RNA 的 RNA 编辑可能导致 mRNA 重新编码，从而增加基因组多样性。 如果编辑发生在内含子中，它可能会产生替代转录本，这些转录本可能会或可能不会转化为蛋白质，可能具有改变的功能。 此外，RNA 编辑可能会影响环状 RNA (circRNA) 的生物发生。 circRNA 周围 Alu 区域的 A-to-I RNA 编辑抑制了 circRNA 的生物发生。 在 miRNA 的种子区域进行 A-to-I 编辑会导致具有功能性后果的重新定位事件。 值得注意的是，与前体信使 RNA 结合的长链非编码 RNA (lncRNA) 可以产生 dsRNA，这是 ADAR1/2 介导的 RNA 编辑的先决条件。 存在于转录本 3'UTR 中的倒置 Alu 的 ADAR1 编辑可能导致 HuR 的展开和随后的募集。 HuR 结合稳定转录物并确保正确加工成蛋白质。


<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/186903974-a9ecf080-c8f7-4b55-8ace-ee7c53d45b54.png" width="1500">
</div>

## 甲基化

### DNA甲基化
#### DNA甲基化酶
DNA甲基化是在DNA甲基转移酶（DNA methyltransferase，DNMTs）的催化下进行的。该反应以S-腺苷甲硫氨酸（SAM）为甲基供体将胞嘧啶核苷酸第5位碳原子进行甲基化生成5-mC

DNMTs家族的成员包括DNMT1、DNMT2、DNMT3a、DNMT3b、DNMT3L等蛋白，它们的结构如下图所示。但请注意，并非上面列出的DNMTs都具有催化DNA甲基化的功能。研究显示，DNMT2的功能主要是催化RNA的甲基化，而DNMT3L并不具备催化活性，所以我们在谈论DNMT的时候，一般指的是DNMT1和DNMT3a/3b。

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/197442179-69533151-175a-4f6f-803b-a02205fe499b.png" width="600">
</div>

虽然DNMT1和DNMT3a/3b这两个蛋白都具有甲基转移酶的活性，但它们对DNA的修饰方式有所不同。

我们知道，DNA是双链结构，双链DNA的任意一条链上的C都可能被甲基化成5-mC。在DNA复制的时候，DNA双链打开形成复制叉，然后执行DNA复制功能的蛋白复合物分别以正义链和反义链分别为模板合成新的双链DNA。因为新合成的这条DNA单链是不含有甲基化的胞嘧啶的，所以，假如模板链的胞嘧啶是甲基化的，那么新生成的DNA双链之中的一条DNA单链甲基化就会“丢失”。

为了解决甲基化丢失的问题，DNMT1就派上了用场——DNMT1负责准确复制DNA甲基化形式，在DNA复制的过程中起着维持甲基化的作用（如下图所示）；而DNMT3a/3b的作用则是在原本任意一条DNA单链都不存在甲基化修饰的位点加上甲基化修饰，即从头（de novo）甲基化。

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/197441816-09366401-7b88-4225-9313-ed4c451fa888.png" width="900">
</div>

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
### RNA甲基化
RNA的甲基化主要发生在N原子上，以及2位的O原子上

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/203678617-bc25e46c-ac0b-4479-9af6-f3b10f18f2c4.png" width="1500">
</div>

#### m6A在mRNA上的作用
m6A的修饰由甲基转移酶复合体（(METTL3–METTL14–WTAP）介导发生；去甲基化由FTO and ALKBH5介导产生

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/203679605-3edfd651-292b-463c-91ac-ba24e234c010.png" width="1500">
</div>

通过直接和间接的方式调控pre-mRNA的剪接

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/203680082-7acfac7a-89ce-413f-9c5c-3fbeee2f564e.png" width="600">
</div>

m6A促进mRNA核输出

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/203680240-3db56e91-6755-4700-a449-d92808cefe08.png" width="600">
</div>

m6A既可以促进mRNA的降解，又可以抑制mRNA的降解

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/203680487-36185df8-8edf-497b-ab48-2939d7063cbd.png" width="600">
</div>

m6A根据其在mRNA中的位置促进或减慢翻译。如果甲基化的腺苷位于5′非翻译区（UTR），真核生物翻译起始因子3（eIF3）的结合会募集43S翻译起始复合物来促进帽非依赖性翻译。如果m6A出现在3′ UTR，YTHDF1或YTHDF3将结合并刺激翻译。然而，如果m6A位于编码区，它可以通过抑制有效的tRNA选择来减慢翻译延伸速率

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/203680552-19f44bc4-7d91-4f50-88f9-688e91a677e0.png" width="600">
</div>

#### m6A在ncRNA上的作用
对于rRNA，无论是大亚基还是小亚基，m6A有助于翻译的增加，同时减缓细胞增殖

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/203681094-bfeda767-6a94-4fa1-814c-21f9c1150950.png" width="600">
</div>

m6A有助于加速miRNA的形成

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/203681263-97ab3bf9-da6d-4fb4-9415-32548b2fd9ff.png" width="600">
</div>

m6A有助于环状RNA的形成，以及促进环状RNA的翻译（Cap-independent translation）

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/203681333-6065b605-fd38-4db9-8f3f-0b911637d809.png" width="600">
</div>

m6A调节小核RNA（snRNA）以促进剪接体装配

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/203681502-0774e6dc-8906-4f30-93b5-d8898ddff889.png" width="600">
</div>

#### 总结一张图
![image](https://user-images.githubusercontent.com/111955215/186906317-e1cb21a2-8ea9-448d-b46c-6f6d5984fab8.png)

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/187030542-76a9b49b-9d59-407b-88fd-05ae8596a5f3.jpg" width="600">
</div>

## 核酸药物
### 基因沉默药物如miRNA siRNA和shRNA
#### 如何递送RNAi药物
![image](https://user-images.githubusercontent.com/111955215/186915771-dc1be989-dd44-4e75-9b47-5d8927c1a85d.png)
![image](https://user-images.githubusercontent.com/111955215/186915917-6b5af86f-4bd7-4521-83b0-b595ad181c69.png)

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
#### shRNA
从结构上看shRNA和miRNA更相似，事实上shRNA在功能上与siRNA更接近。shRNA在细胞内被Dicer酶切割后形成siRNA，通过siRNA途径行使干扰功能，而miRNA则是通过另一条不同的途径调控目标基因。
shRNA实际上是通过载体构建在体内获取siRNA的一种方式，两者结构本质上是相同的，但在功能上有所差异。
shRNA是可以克隆至表达载体并表达双链siRNA的RNA分子，包括两个短反向重复序列，中间由一茎环序列分隔，形成发夹结构，由polⅢ启动子控制。相对于siRNA，shRNA在细胞核中合成，进一步加工并运输到细胞质中，然后进入RISC发挥活性。miRNA的合成与成熟研究为shRNA的合成，特别是基于miR-30的shRNA的合成提供了基础。

![image](https://user-images.githubusercontent.com/111955215/186809306-52a2795f-dcab-4c7e-b98a-04efbba9b2a0.png)
### ASO反义核苷酸药物
反义寡核苷酸(ASOs)被定义为化学合成的寡核苷酸，通常长度为12-30个核苷酸，目的是通过Watson-crick碱基配对规则与RNA结合。
![image](https://user-images.githubusercontent.com/111955215/186809553-4536089e-8f7c-4394-b43c-3b0f0409740c.png)

* 占位机制：通过与细胞核内的pre-mRNA互补，导致poly-A的尾不能正常形成或剪接成熟不能进行；通过与细胞核外的成熟mRNA结合，导致其翻译不能正常进行

![image](https://user-images.githubusercontent.com/111955215/186810198-feeab0e5-b548-4c7f-8d9b-efdec47122e0.png)

* RNA降解机制：通过招募RNase H1或Argonaute 2(Ago 2)降解RNA
 
![image](https://user-images.githubusercontent.com/111955215/186810609-721a4f4b-a844-4c1e-9fa2-e89e4e219783.png)
* 抵抗miRNA的降解：通过与miRNA形成base pair抵抗其降解作用，此机制为上调

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/186899924-ca162588-0fcb-40eb-90b4-8bb6bd1f97d5.png" width="1500">
</div>

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

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/186900304-00185b3f-14e7-4137-ab71-f8fad9ddfcc1.png" width="1500">
</div>

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

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/186900444-cc8bd421-ec01-48f2-ae78-45a6743c7b8e.png" width="1500">
</div>

## 免疫检查点/immune checkpoint
### PD-1/PD-L1
![image](https://user-images.githubusercontent.com/111955215/186914841-7a873cf3-b747-4e3b-8e2b-1f375d6ae6bd.png)

![image](https://user-images.githubusercontent.com/111955215/186914892-cedea0fb-e486-4835-935b-71d913d1ff47.png)

![image](https://user-images.githubusercontent.com/111955215/186914950-2f9e4484-2876-4ff6-adbf-c55163f808b2.png)

#### The difference between PD-1 and PD-L1
在实际试验中，人们发现达到同样的抑制效果PD-L1的剂量必须非常高，这就导致PD-L1的成本远远高于PD-1。PD1的剂量，大家差不多就是200mg 3周注射一次；PD-L1的剂量，阿斯利康的PDL1 Durvalumab剂量是1500mg 4周一次，故一旦药物价格面临着下行压力，PD-L1商业化价值远远低于PD1。

#### PD-1和PD-L1现在存在的问题
其实除了成本难以下降之外，PD-1的给药方式还是以静脉给药为主，每2~3周一次，虽然现在纳米抗体可以实现皮下注射，但是易用性远不及口服小分子药物。患者依从性：口服＞皮下注射＞静脉注射

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/186900623-5a9379c2-0ac2-4e66-ba1e-5c6122d84fc8.png" width="1500">
</div>

## crispr系统
DNA target recognition requires both base pairing to the crRNA sequence and the presence of a short se-quence (PAM) adjacent to the targeted sequencein the DNA 

![image](https://user-images.githubusercontent.com/111955215/187072595-a18aac54-cdcd-46a2-a06b-81debac643fa.png)

天然的crispr系统和人工的区别：**人工的gRNA是连在一起的，可以用一条序列表达**

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/187072598-c0159446-7980-4fc5-af25-ed4975afad6d.png" width="800">
</div>

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

<div align=center>
<img src="https://user-images.githubusercontent.com/111955215/186900804-41616c82-57db-4bfd-af7a-fcd2b3e2f012.png" width="1500">
</div>

## Phage Display
噬菌体展示技术有多种分类标准。根据噬菌体的不同，可以分为M13、T7、T4、λ等多种体系；根据载体的不同，可以分为噬菌体载体（True Phage）和噬菌粒载体（Phagemid）；根据文库的不同，可以分为随机肽库、cDNA文库、抗体文库、蛋白质文库等。
抗体库的筛选是指从抗体库中筛选出针对某一抗原的特异性抗体，是获得高亲和力抗体过程中的关键环节。单克隆抗体性质存在千差万别，需根据不同的单抗制定严格的筛选条件，一般分为经典筛选法和新型筛选法。
### 经典筛选法
主要为固相筛选法和液相筛选法，用于抗原性质明确的抗体筛选。固相筛选法通过包被在酶标板或其他固相介质上的抗原富集高亲和性的噬菌体；液相筛选法(如下图)是将生物素化的抗原包被在与亲和素偶联的磁珠或琼脂糖上，进行抗原特异性结合的方法。通过多次筛选，抗原得到高亲和力的噬菌体。
![image](https://user-images.githubusercontent.com/111955215/186395522-6735bf29-58da-4889-9b65-70f5731ee7f6.png)
### 新型筛选法
当抗原无法纯化或性质不明时，就需要开发新的筛选方法，用于抗体库的建立。目前比较成熟的有细胞筛选法、组织切片或体内筛选法、选择感染筛选法、蛋白质芯片筛选法等。
细胞筛选法可以维持抗原和抗体的天然构象，多用于肿瘤细胞抗体筛选，还适用于细胞表面受体及抗原鉴定。但由于细胞膜表明成分复杂，会增加非特异性结合，而多次筛选又容易丢失特异性结合的抗体，因此限制了此方法的应用，并且在此方法基础上开发了扣除筛选、竞争筛选、内化筛选等方法。
