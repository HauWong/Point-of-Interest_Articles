> 共12篇

- **2014 - Fine-resolution population mapping using OpenStreetMap points-of-interest**
    - **内容**：本文利用建筑物足迹和POI数据作为辅助数据来估算城市人口在建筑物尺度上的分布。
    - **方法**：
        1. 首先利用土地利用与土地覆盖分类数据将城市人口分布（以区为单位）数据进行分割；
        2. 采用Surface volume integration方法将人口数据插值为以网格单元为基本单元的人口分布，该方法基于相关POI的空间分布来估算人口，其中POI数据经过ID3决策树分类；
        3. 最后利用建筑物足迹数据来计算每个建筑物的人口密度。
- **2018 - Dynamic assessments of population exposure to urban greenspace using multi-source big data**
    - **内容**：利用多源数据（遥感数据、社交媒体数据）动态评估城市绿地开放程度。
    - **方法**：
        1. 数据预处理：对POI进行选择和标注，对夜间灯光影像进行月平均处理，将腾讯MPL数据转换为栅格形式；
        2. 利用一种自适应的方法处理POI和夜间灯光数据，定义城市区域；
        3. 从高分辨率遥感影像中提取城市绿地区域；
        4. 对不同尺度下的绿地人均开放程度进行动态评估。

- **2018 - Temporal and Spatial Variation Characteristics of Catering Facilities Based on POI Data: A Case Study within 5th Ring Road in Beijing**
    - **内容**：本文利用POI数据基于DBSCAN、核密度估计和词云分析，从宏观、中观和微观三个维度分析了北京市2012、2014和201年餐饮点和餐饮集群的结构类型和时空演化特征。

- **2018 - Using points-of-interest data to estimate commuting patterns in central Shanghai, China - Mengya Li**
	- **内容**：本文利用兴趣点数据来估计就业地点，并采用基于重力的模型来估计上海市中心的通勤模式。
	- **方法**：
		1. 对POI进行分级分类，通过调查重要POI点的职工以估算基于二级POI类型的就业数量，然后按类别统计每个城区的POI数量，并基于此计算得到在每500m的格网内的就业数量，绘制就业密度图；
		2. 分别以个人驾车时间与公共驾驶时间的最小值估算城区中心之间的旅行时间矩阵；
		3. 采用TSME程序和重力模型计算城区间的交通流量，进而估算通勤距离，分析通勤模式。

- **2019 - Exploration on the spatial spillover effect of infrastructure network on urbanization: A case study in Wuhan urban agglomeration - Chen Zeng**
	- **内容**：本文通过对2005年和2015年武汉城市空间模型的建模，提出基于道路网和基于POI两种假设探讨了基础设施网落对城市化的空间溢出效应。
	- **方法**：
		1. 第一种假设认为，城市化的空间溢出效应是由基于线的道路网产生，把道路网分为高速公路、国道、省道和县道四种类别，并基于空间句法理论对每种类别计算积分值，使用所有类别的平均值来生成道路网的全局积分值；
		2. 第二种假设认为空间溢出效应是由点设施引起的，对POI进行提前分类，并计算密度；
		3. 将路网积分值和POI密度嵌入到重力模型中，得到空间权重矩阵，进行空间建模。

- **2019 - Understanding the impact of built environment on metro ridership using open source in Shanghai - Dadi An**
	- **内容**：本文采用兴趣点数据来研究影响上海地铁客流量的物理因素。

- **2019 - Spatiotemporal distribution characteristics and mechanism analysis of urban population density: A case of Xi'an, Shaanxi, China Jingang - Jingang Li**
	- **内容**：本文基于百度热力图数据和城市POI数据，采用人口密度指数（PDI）、空间相关指数（SCI）和最小二乘法模型分析了西安市城市空间人口密度的时空分布特征及其变化规律。

- **2020 - Visualizing and exploring POI configurations of urban regions on POI-type semantic**
    - **内容**：目前研究**POI配置**的方法和应用主要针对不同类型的POI分别进行分析，忽略了类型之间隐含的语义关系。本文考虑类型间的语义关系提出一种新型POI配置可视化和探索框架。
    - **方法**：
        1. 依据POI在空间上的邻居采用Word2Vec方法进行POI类型嵌入；
        2. 通过降维技术将POI类型嵌入映射到二维语义空间，其中相似或相关的类型间彼此接近；
        3. 以POI类型语义空间作为基本图，根据每个区域中不同的POI类型绘制POI配置专题图。
- **2020 - Identifying and evaluating poverty using multisource remote sensing and point of interest (POI) data: A case study of Chongqing, China**
    - **内容**：本文以重庆为研究区，结果多种数据来源（夜间灯光数据、数字高程模型、归一化植被指数和POI数据）分析贫困问题。
    - **方法**：
        1. 基于地表坡度（从DEM中获得）、人类居住指数（HSI，从夜间灯光数据和NDVI中得到）、POI密度和POI cost distance提出一种综合的贫困指数（CPI）；
        2. 通过简单的视觉比较和社会经验数据来验证CPI；
        3. 最后利用CPI从多尺度视角评估重庆市的贫困分布状况。

- **2020 - Analysis on spatiotemporal urban mobility based on online car-hailing data - Bin Zhang**
	- **内容**：本文利用在线打车数据，识别出高出行强度区域的分布，并分析出行强度与兴趣点之间的相关性。
	- **方法**：
		1. 利用规则格网将城市划分为若干区块，经纬度尺度为0.002度，并统计每个区块的网约车接放数量；
		2. 将POI分为13个类型，并统计每个区块中各类型POI的数量；
		3. 基于上述数据，确定每个区块的出行强度和POI密度等级；
		4. 采用有序逻辑回归分析出行强度与POI密度之间的关系。

- **2020 - Understanding the spatial organization of urban functions based on co-location patterns mining: A comparative analysis for 25 Chinese cities - Yimin Chen**
	- **内容**：以往的研究主要集中在城市功能类型的推断上，而从活动的空间共现角度对城市功能组织的认识却很少。为了解决这一问题，本文提出了一种利用兴趣点数据挖掘城市活动共定位模式（co-location patterns, CPs）的新方法。
	- **方法**：
		1. 利用城市范围对POI数据进行筛选；
		2. 对每个城市的POI采用CPs挖掘算法（文中有详细介绍）；
		3. 基于生成的CPs，度量城市功能空间组织的显著性。

- **2020 - Investigating the impacts of built environment on traffic states incorporating spatial heterogeneity - Yingjiu Pan**
	- **内容**：本文研究影响工作日晚高峰期间交通状态的潜在因素，提出一种基于地理加权回归的交通状态空间异质性建模方法。
	- **方法**：
		1. 研究单元为TAZ（Traffic Analysis Zone），计算每个TAZ交通状态指数（TSI），将POI分为三个类型：公共及商业建筑、住宅和景点，收集道路特征数据和公共交通设施数据；
		2. 设计解释变量：选择公交站点数、地铁站点数、公交线路数、地铁线路数作为候选解释变量；
		4. 采用皮尔森相关性分析和方差膨胀因对候选解释变量进行多重共线性检验；
		5. 通过莫兰指数对各变量进行空间自相关检验；
		6. 建立地理加权回归模型，分析解释变量对交通状况的影响。 