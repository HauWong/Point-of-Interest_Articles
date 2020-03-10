> 共5篇

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