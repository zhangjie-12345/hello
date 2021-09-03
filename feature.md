# hello
基于华为Taishan服务器的微型生物大数据分析课
软件列表
整理人：倪家豪
更新日期：2021.1.27

*本软件列表提供下载安装方式，使用软件请务必引用原始文献。

	Ghelper
软件用途：无需挂vpn即可使用Google搜索引擎。
软件下载地址： 
http://googlehelper.net/
插件安装：
1.在网址栏输入: chrome://extensions/ 。
2.点击 “添加已解压的扩展程序”,如果没有，打开右边“开发者模式”开关。 
3.选择本次下载包里的 ghelper_source 目录并确认，
4.点击打开插件图标，注意需要注册插件账号，登录账号后就可以使用google了。 

	VMware
VMware16pro，以软件之身模拟硬件系统构建虚拟机。
在官网https://www.vmware.com/cn.html注册后下载或下方网盘中点击下载：
	  网盘下载：链接：https://pan.baidu.com/s/1dHaWQJ2rh1OG8EGs6sd_yg			  
提取码：1234 
	激活密钥：ZF3R0-FHED2-M80TY-8QYGC-NPKYF
			  YF390-0HF8P-M81RQ-2DXQE-M2UT6
			  ZF71R-DMX85-08DQY-8YMNC-PPHV8
密钥摘自：VMware16Pro永久激活key密钥亲测可用 - 谷粒源-分享最精品的资源,快乐的源泉就在这里等你发现! (gulicms.com)

	CentOS 7虚拟机
CentOS 7，免费的开源的操作系统 ，CentOS（Community Enterprise Operating System，）是Linux发行版之一。
	镜像下载：官网CentOS-7-x86_64-DVD-2009.iso (aliyun.com)下载或下方网盘链接：
网盘下载：链接：https://pan.baidu.com/s/1dHaWQJ2rh1OG8EGs6sd_yg
			  提取码：1234

	R
R是用于统计分析、绘图的语言和操作环境。免费开源，是用于统计，计算和制图的优秀工具。
下载地址：
https://mirrors.tuna.tsinghua.edu.cn/CRAN/bin/windows/base/ 
Rtools下载地址：
https://cran.r-project.org/bin/windows/Rtools/rtools40-x86_64.exe
有关R无法调用stats的解决方法：
https://blog.csdn.net/princess_guo/article/details/108842155

	Rstudio
RStudio是R编程语言的集成开发环境，比R本体更加易于操作和可视化。
下载地址：https://rstudio.com/products/rstudio/download/

	Anaconda
Anaconda是一个包含180+的科学包及其依赖项的发行版本。可以便捷的安装和升级包及其依赖项。可以在计算机中便捷地创建、保存、加载和切换环境。
Miniconda是Anaconda的缩略版。
Bioconda是一个频道，专门提供生物信息学软件下载。
Conda是一个包管理工具，本身也是一个命令。Anaconda中包含Conda。
原始网址：https://anaconda.org/
安装命令：
#下载安装程序或寻找助教拷贝。提前下载好的可直接拖拽入虚拟机文件目录#
wget https://repo.anaconda.com/archive/Anaconda3-2020.11-Linux-x86_64.sh
#安装时，条款全部接受即可#
su  #进入root用户，需输入正确root密码并回车
bash Anaconda3-2020.11-Linux-x86_64.sh
#验证#
bash
#查看conda版本#
conda -V
#启动，如果在虚拟机用户名前出现(base)则表示成功进入Conda#
conda activate
#关闭#
conda deactivate
#添加常用镜像地址#
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/free/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/main/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/bioconda/
conda config --set show_channel_urls yes

补充：
Conda install ***(软件名)  #安装***软件
Conda uninstall ***(软件名)   #卸载***软件
Anaconda search -t conda show ***(软件名)    #安装指定版本的包
#运行后显示版本信息
Anaconda show $$$$/***(版本信息)#显示指定安装包的安装源
直接运行最后一句话即可

Anaconda卸载
1、	安装anaconda-clean package 
2、	打开anaconda Prompt，输入命令行 #conda install anaconda-clean
3、	接着输入命令行进行卸载   #anaconda-clean –yes
4、	对于anaconda3，直接运行其安装目录下的Uninstall-Anaconda3.exe
	git
下载工具。
安装命令：
conda install git -y

	BWA 
BWA 是用于将 DNA 序列比对到大的参考基因组的软件包。
原始网址：https://github.com/lh3/bwa
版本：0.7.17-r1188
安装命令：
conda install bwa -y

	Samtools
Samtools 是一个用于操作 sam 和 bam 文件的工具合集。
原始网址：http://www.htslib.org/
版本：1.9
安装命令：
conda install samtools=1.9 -y
ln -s libcrypto.so.1.1 libcrypto.so.1.0.0

	cap3
Cap3是一款可以自动拼接Sanger双端测序序列的软件。
原始网址：http://doua.prabi.fr/software/cap3
版本：02/10/15
安装命令：
conda install cap3 -y

	fastp
fastp可以自动识别序列接头并进行修剪。
原始网址：https://github.com/OpenGene/fastp/
版本：0.20.1
安装命令：
conda install fastp -y

	FastQC
FastQC可以用来查看序列质量。
原始网址：http://www.bioinformatics.babraham.ac.uk/projects/fastqc/
版本：0.11.9
安装命令：
conda install fastqc -y

	SeqMan
SeqMan是一款手动拼接Sanger双端测序序列的软件，属于DNAstar软件包，正版需要付费。
原始网址：https://www.dnastar.com/
安装方法：助教分享

	Nanopack
Nanopack是一个长测序序列处理和分析脚本合集。
原始网址：https://github.com/wdecoster/nanopack
安装命令：
方法1：
yum install zlib-devel
pip install nanopack
方法2：
conda create -y -n nanopack
conda activate nanopack
conda install -c bioconda nanoqc nanoplot  nanostat  nanofilt
conda deactivate nanopack
	BWA-MEM2
BWA-MEM2是BWA的优化版本。
原始网址：https://github.com/bwa-mem2/bwa-mem2
版本：2.1
安装命令：
conda install bwa-mem2 -y

	minimap2
针对长测序序列的比对软件。
原始网址：https://github.com/lh3/minimap2
版本：2.17-r941
安装命令：
conda install minimap2 -y

	java SE8
可以自动配置环境变量，用于Mauve等需要java环境的软件。
原始网址：https://www.oracle.com/java/technologies/javase-downloads.html
版本：15.02
安装：网页下载对应版本进行安装。

	Mauve
原始网址：http://darlinglab.org/mauve/download.html
版本：2.4.0
安装：http://darlinglab.org/mauve/download.html

	Trimmomatic
Trimmomatic可以去除测序序列接头。
原始网址：http://www.usadellab.org/cms/index.php?page=trimmomatic
版本：0.39
安装命令：
conda install trimmomatic -y

	Unicycler
Unicycler：调用并优化SPAdes序列组装，自动使用 pilon 等软件进行纠错，支持长reads、短reads各自的组装及长短reads的混合组装。
原始网址：https://github.com/rrwick/Unicycler#quick-usage
版本：0.4.8
安装命令：


	Quast
进行基因组组装结果评估。
原始网址：http://quast.sourceforge.net/
版本：5.0.2
安装命令：
wget https://downloads.sourceforge.net/project/quast/quast-5.0.2.tar.gz
tar -xzf quast-5.0.2.tar.gz
cd quast-5.0.2
python setup.py install_full
quast.py

	BUSCO
原始网址：https://gitlab.com/ezlab/busco
版本：
安装命令：
conda create -n busco -c bioconda -c conda-forge busco=5.0.0
#进入busco环境后再使用busco
conda activate busco
#退出busco环境
conda deactivate busco

	Canu
专门为错误率高的长读长设计的组装软件。
原始网址：https://github.com/marbl/canu
版本：
安装命令：

	Spades
功能强大，能够组装多种类基因组，如宏基因组、线粒体基因组的组装软件。
原始网址：https://github.com/ablab/spades
版本：v3.14.1
安装命令：
conda install spades -y

	Racon
Racon可以对未纠错的长序列组装得到的基因组进行纠错。
原始网址：https://github.com/isovic/racon
版本：v1.4.20
安装命令：
conda install racon -y

	Pilon
自动改善draft genome质量，和检测突变和大尺度的删除。
原始网址：https://github.com/broadinstitute/pilon/wiki
版本：1.23 Mon Nov 26 16:04:05 2018 -0500
安装命令：
conda install Pilon -y

	Trinity
组装处理 Illumina RNASeq，后可用于注释及表达量差异分析等的数据
原始网址：https://github.com/trinityrnaseq/trinityrnaseq
版本：2.8.5
安装命令：
  conda creat -n trinity
conda activate trinity
conda install trinity
conda update trinity
bash

	Hisat2
用于RNA测序序列的比对。
原始网址：https://daehwankimlab.github.io/hisat2/
版本：2.2.1
安装命令：
conda install hisat2

	StringTie 
将RNAseq比对到潜在的转录本。
原始网址：http://ccb.jhu.edu/software/stringtie/
版本：2.1.4
安装命令：
conda install stringtie -y

	Braker2
原始网址：http://exon.gatech.edu/GeneMark/braker.html
版本：
安装命令：
conda create -n braker2
conda install braker2
bash
需要GeneMark-ES：注册后下载对应的软件包及key文件
注意：如果没有这个Key文件就不能使用，并且Key文件需要实时更http://exon.gatech.edu/GeneMark/license_download.cgi

cp -r /root/anaconda3/envs/braker2/config/ /absolute_path_to_user_writable_directory/
export AUGUSTUS_CONFIG_PATH=/absolute_path_to_user_writable_directory/config

	Augustus
Braker2利用conda install 安装时会自带安装比较老版的Augustuts的软件，如果报错，可以在Augustuts官网中下载最新版的脚本，把里面script脚本替换。目前可能会有三个脚本报错，或者利用conda install 安装一个新版的Augustuts
原始网址：http://bioinf.uni-greifswald.de/augustus/
版本：3.3.3
安装命令：
conda activate braker2
conda install augustus
bash

	tRNAscan-SE
寻找tRNA基因。
原始网址：http://lowelab.ucsc.edu/tRNAscan-SE
版本：2.0.7
安装命令：
    conda install trnascan-se -y

	hmmer      
原始网址：http://www.cbs.dtu.dk/services/RNAmmer/   
版本：2.2
安装命令：
   wget http://eddylab.org/software/hmmer/hmmer-2.2g.tar.gz           tar zxf hmmer-2.2g.tar.gz                                        cd hmmer-2.2g/           ./configure --prefix=/home/wyh/software/hmmer-2.2g           mkdir -p /home/wyh/software/hmmer-2.2g/man/man1/ /home/pj/software/hmmer-2.2g/bin           make 注册下载：rnammer软件           tar zxf rnammer-1.2.src.tar.gz -C rnammer-1.2            perl -p -i -e 's/(my \$INSTALL_PATH).*/$1 = \"\/home\/wyh\/software\/rnammer-1.2\";/' /home/wyh/software/rnammer-1.2/rnammer perl -p -i -e 's/^(\s+\$HMMSEARCH_BINARY).*/$1 = \"\/home\/wyh\/software\/hmmer-2.2g\/bin\/hmmsearch\";/'

	aspera-cli
原始网址：https://www.ibm.com/products/aspera/downloads
版本：3.9.1
安装命令：
conda create -n download 	   
conda activate download  conda install -y -c hcc aspera-cli 		
conda install -y -c bioconda sra-tools  bash

	sra-tools
下载工具。
安装命令：见上方aspera-cli
	GATK
一个基因组分析工具包。
原始网址：https://gatk.broadinstitute.org/hc/en-us
版本：4.1.9.0
安装命令：
wget https://github.com/broadinstitute/gatk/releases/download/4.1.9.0/gatk-4.1.9.0.zip

	QIIME 2
QIIME 2是一款强大、可扩展和去中心化的微生物组分析平台，强调数据分析透明。QIIME 2可以使研究者从原始DNA序列开始分析，直接获取出版级的统计和图片结果。
原始网址：https://docs.qiime2.org
版本：2020.11
安装命令：
wget -c http://210.75.224.110/github/QIIME2ChineseManual/2020.11/qiime2-2020.11-py36-linux-conda.yml
conda env create -n qiime2 --file qiime2-2020.11-py36-linux-conda.yml

	FAPROTAX
进行生物学功能注释。
原始网址：https://pages.uoregon.edu/slouca/LoucaLab/archive/FAPROTAX/lib/php/index.php
安装命令：
wget https://pages.uoregon.edu/slouca/LoucaLab/archive/FAPROTAX/SECTION_Download/MODULE_Downloads/CLASS_Latest%20release/UNIT_FAPROTAX_1.2.4/FAPROTAX_1.2.4.zip
unzip FAPROTAX_1.2.4.zip

	KneadData
一个用于宏基因组测序数据，特别是微生物组实验数据的质量控制的工具。
原始网址：https://huttenhower.sph.harvard.edu/kneaddata/
版本：0.9.0
安装命令： 
sudo pip install kneaddata

	HUMAnN3
原始网址：https://huttenhower.sph.harvard.edu/humann
版本：v3.0.0.alpha.3
安装命令：
conda config --add channels biobakery
conda install humann -c biobakery
humann_test
首次运行会自动下载MetaPhlAn3数据库，其他数据库下载：
humann_databases --download chocophlan full /path/to/databases --update-config yes
humann_databases --download uniref uniref90_diamond /path/to/databases --update-config yes
humann_databases --download utility_mapping full /path/to/databases --update-config yes

	MetaPhlAn3
用于从宏基因组测序数据中分析微生物群落的组成。
随HUMAnN3一同安装。

	hclust2
可用于宏基因组的绘图。
原始网址：https://github.com/SegataLab/hclust2
版本：1.0.0
安装命令：
	conda install -c bioconda hclust2

	GraPhlAn
可生成高质量的分类和系统发育树的圆形图示。
原始网址：http://huttenhower.sph.harvard.edu/GraPhlAn
版本：1.1.4 (16 July 2020)
安装命令：
	git clone https://github.com/biobakery/graphlan.git
	export PATH=`pwd`/graphlan/:$PATH

	STAMP
用于分析微生物分类和功能谱，可以进行统计和绘图。
原始网址：https://beikolab.cs.dal.ca/software/STAMP
版本：2.1.3
安装命令：
下载网址https://beikolab.cs.dal.ca/software/STAMP 选择合适的windows版本进行下载

	MUSCLE
原始网址：http://www.drive5.com/muscle
版本：3.8.31
安装命令：
wget http://www.drive5.com/muscle/downloads3.8.31/muscle3.8.31_i86linux64.tar.gz
tar -xvf muscle3.8.31_i86linux64.tar.gz

	Gblocks
一款自动去除gap的软件。
原始网址：http://www.vardb.org/vardb/analysis/gblocks.html
版本：0.91b
安装命令：
conda install gblocks


	ALTER
便捷的格式转换软件。
原始网址：
版本：1.3.4
安装命令：
conda install openjdk
conda install maven
git clone https://github.com/sing-group/ALTER.git
cd ALTER
mvn package

	PhyML
使用PHY格式文件构建ML树。
原始网址：http://www.atgc-montpellier.fr/phyml/
版本：3.1
安装命令：
wget http://www.atgc-montpellier.fr/download/binaries/phyml/PhyML-3.1.zip
unzip PhyML-3.1.zip

	Paup4
可以进行模型计算。
原始网址：http://phylosolutions.com/paup-test/
版本：4
安装：
http://phylosolutions.com/paup-test/paup4-setup.msi
双击安装程序进行安装

	Adobe Illustrater
Al是大数据可视化的一种便捷、高效的工具，可以将各种信息进行重新整理、加工和美化后进行可视化。
原始网址：https://www.adobe.com/cn/products/illustrator.html
安装：
https://pan.baidu.com/s/1uyvNrrVtaiNV_Rgs_Q533A 
提取码：1234

R包安装
以下为课程中用到的R包，需要进行安装。
if (!requireNamespace("BiocManager", quietly = TRUE)) install.packages("BiocManager") 
BiocManager::install("DESeq2")
#程序包安装命令（当提示所需安装包不适用于当前R版本时，可使用上述命令
install.packages("")
#使用上述程序包安装命令安装以下包：
	BiocManager
	reshape
	DESeq2
	gridExtra
	readxl
	zoo
	Rcpp
	devtools
	baidumap
	REmap

以下网页需要进行注册：
	GenSAS
GenSAS（Genome Sequence Annotation Server）是一个基于网页的基因组序列注释工具。
https://www.gensas.org/
	RAST
RAST (Rapid Annotation using Subsystem Technology)是一个能够对完整或较为完整基因组进行注释的在线工具。
https://rast.nmpdr.org/
	iTOL
iTOL全称Interactive Tree Of Life，是一种显示、注释和管理系统发育树的在线工具。
https://itol.embl.de/

