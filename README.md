# 一、赛题	
   包裹X光限制品监测作为日常包裹物流行业及安防行业的重要环节，承担着防止易燃易爆等危险品进入货运渠道，管理刀具等特殊货运物品，监测毒品等国家重点违禁品偷运等工作。随着线上购物的普及和快速发展，线上物流包裹数量已经远超人工可以处理的范围，给物流包裹监管带来了巨大挑战。
本次比赛着眼于此，邀请选手针对给出的限制品种类，利用X光图像及标注数据，研究开发高效的计算机视觉算法，监测图像是否包含危险品及其大致位置。通过自动化监测包裹携带品算法，降低漏检风险及误报率，提升危险品管理效率。本次比赛是一次未来物流及安防行业的有益尝试，对行业未来发展有着不可估量的价值。
赛题链接：https://tianchi.aliyun.com/competition/entrance/231710/information

# 二、程序说明
1、采用MaskRCNN_benchmark框架，框架的安装依照install.md进行;   
2、test_save.py文件的作用是生成提交的json文件;    
3、datasetprocess文件夹下是对数据集的处理文件;    

# 三、使用MaskRCNN_benchmark训练自己的数据集
1、将数据集放置在datasets/coco/文件夹下，具体路径如maskrcnn_benchmark\config\paths_catalog.py文件所示;   
2、使用tianchi_train_mutgpus.sh进行多GPU训练，使用tianchi_train_singlegpus.sh进行单GPU训练;  
