> 共13篇

- **2012 - Discovering Regions of Different Functions in a City Using Human Mobility and POIs**
    - **内容**：本文提出一个DRoF框架，该框架整合了POI和不同地块间的人口流动数据（出租车轨迹），并利用主题模型识别城市中不同的功能区。作者认为，仅用POI无法反映区域之间的相互作用，因此引入人类活动数据即出租车轨迹数据来表达区域间的交互（人们从如果从相似的区域前往某两个区域，或者从某两个区域前往相似的区域，那么这两个区域更有可能具有相似的功能）。
    - **方法**：
        1. 利用道路网数据将城市分割为众多地块；
        2. 定义了两个迁移立方体，用以表达人们离开出发地和到达目的地的活动模式，立方体的三个维度分别为：地点、地点和时间段；
        3. 将迁移模式视作单词、POI视作元数据、功能视作主题，区域即文档，然后采用一种基于LDA和狄利克雷多项式回归的主题模型来提取区域的主题；
        4. 在利用K-Means方法针对众多区域的主题分布进行聚类，将所有区域聚类为k个功能区；
        5. 由于功能区的功能在总体上并不是均匀分布的，核心功能可能会跨越多个区域，并且有不规则的形状，因此利用人类活动模式进行核密度分析来估计每个功能区的功能强度。
        6. 综合考虑POI类型、活动模式和功能强度对区域进行标注。
- **2013 - Automated identification and characterization of parcels (AICP) with OpenStreetMap and Points of Interest**
    - **内容**：本文利用OSM道路网络划分城市地块，并用POI数据来推断地块特征，实验面向全国297个城市。
    - **方法**：
        1. 地块划分：先利用OSM道路数据进行分块，得到不同的地块，再用行政边界进行叠加，以确定地块所属的城市；
        2. 地块特征：土地利用密度——地块内/附近的POI数量，并将密度归一化至0-1之间，以更好地比较城际和城市密度；
        3. 城市地块选取：采用一种基于向量的元胞自动机模型识别城市中的块；
        4. 确定地块功能和土地利用结构：以地块中的主导POI类型确定地块功能，并计算一个混合指数来表示土地利用的混合程度。
- **2015 - Mapping Urban Land Use by Using Landsat Images and Open Social Data**
    - **内容**：本文结合POI数据与Landsat影像，以特征向量的相似度为标准判别城市土地利用类型。介绍了整体流程、POI数据的处理过程、及城市土地利用类型分类标准等内容。
    - **方法**：
        1. 首先利用道路网将研究区域分隔为众多地块；
        2. 将这些地块分为建筑区和非建筑区两种类型，这些地块的功能将由其与预先收集的训练样本之间的归一化特征距离（相似性）来决定；
        3. 建筑区的相似性测度由两种类型的特征决定，即社会特征和物理特征，分别对10种POI数据进行核密度分析并归一化，得到10种的社会特征；从多时相的Landsat影像获取两种物理特征；
        4. 非建筑区的相似性则由其上的主导地物覆盖类型决定；
        5. 最终，将两种区域的分类结果结合
- **2015 - An integrative method for mapping urban land use change using “geo-sensor” data**
    - **内容**：本文结合多源数据（遥感影像与社交媒体数据）进行城市土地利用类型变化分析。
    - **方法**：
        1. 将Landsat影像进行土地覆盖类型分类；
        2. 根据POI类型所代表的面积大小划分POI等级，进行初步土地利用类型分类；
        3. 结合Twitter数据和POI将居住区二级土地利用类型细分。
- **2017 - Hierarchical semantic cognition for urban functional zones with VHR satellite images and POI data - Xiuyuan Zhang**
    - **内容**：构建了一种层级分类框架，依次从场景的视觉特征、对象类别、空间分布模式和区域功能等四个层次对场景进行语义表达，实现功能分类，其中在对象类别层次引入POI数据，以加入影像无法描述的社会信息。
- **2017 - Classifying urban land use by integrating remote sensing and social media data**
    - **内容**：结合遥感影像、POI数据、腾讯实时用户密度和OSM数据，采用词袋模型和主题模型进行逐步的特征抽象表达，最终用SVM分类器对城市地块的土地利用类型进行分类。
    - **方法**：
        1. 特征提取：通过窗口滑动的方式从遥感影像中提取光谱特征、纹理特征、空间特征和SIFT特征；
        2. 词袋构建：利用K-Means聚类器将上述影像特征抽象为视觉单词，并利用K-Means将用户密度数据抽象为单词，并统计POI数据类型，最终构建包含以上几种数据的词袋模型；
        3. 分块：利用OSM数据将实验区的上数据分为多个地块得到样本；
        4. 主题抽象：利用主题模型将词袋中的数据进行主题分析，得到固定的几个主题的分布向量；
        5. 分类：利用SVM分类器对抽象后的主题分布向量分类。
- **2017 - Extracting urban functional regions from points of interest and human activities on location-based social networks**
    - **内容**：基于POI类型的共现模式结合用户在社交网络上的签到数据建立了一种统计框架，利用LDA主题模型从中得到具有语义特性的主题并以此分类功能区。并且将主题分布应用到寻找特征相似的地区方面，具体有两种应用手段：1. 以某地区的最大概率的主题来寻找与之相似的地区，2. 以某地区的所有主题分布来寻找与之相似度高的地区
    - **方法**：
        1. 利用签到数据来评价POI类型的流行性，重新计算POI类型的数量；
        2. 利用LDA模型对POI数据进行分析，对于每个区域都得到一个K维的主题向量，表达的是该区域的主题语义；
        3. 采用两种方法对主题向量进行聚类：K-Means聚类、狄洛尼三角网空间约束聚类（Delaunay triangulation spatial constraints clustering methods），得到功能区分类。
- **2017 - The Combined Use of Remote Sensing and Social Sensing Data in Fine-Grained Urban Land Use Mapping: A Case Study in Beijing, China**
    - **内容**：本文从OSM道路网划分的城市地块中得到的四种属性：光谱/纹理特征、景观指标、POI和微博数据特征。采用随机森林方法对城市土地利用类型进行分类。通过对结果的分析发现，该方法对开放性用地和住宅用地的分类效果相对较好，而对机构用地的分类效果不佳。景观指标是开放性用地识别的最重要的属性，而光谱/纹理特征对识别机构和居住地块更重要，对商业地块的识别则更依赖于景观指标和社交媒体数据（POI及微博数据），而对光谱/纹理数据的依赖较弱。
    - **方法**：
        1. 利用OSM道路网划分地块；
        2. 从遥感影像中提取光谱/纹理特征，并根据土地覆盖图中获得景观指标；
        3. 计算POI的密度和空间分布模式，以及微博数据的密度；
        4. 采用随机森林模型进行分类，并用精度平均下降这一指标进行特征重要性分析。
- **2017 - Sensing spatial distribution of urban land use by integrating points of interest and Google Word2Vec model**
    - **内容**：本文将Word2Vec模型与POIs相结合，在比较精细的尺度上识别城市用地类型，Word2Vec是一种深度学习语言模型，能根据上下文关系将单词映射到高维向量空间。
    - **方法**：
        1. 利用百度POI和TAZ（Traffic Analysis Zone）建立TAZ-POI语料库；
        2. 并利用Word2Vec模型将TAZ-POI语料库量化为特征向量，TAZ向量是通过计算内部POI向量和的平均值求得；
        3. 使用一种基于随机森林的监督分类方法对TAZ向量进行计算得到用地类型。

- **2018 - Social functional mapping of urban green space using remote sensing and social sensing data**
    - **内容**：本文提出一种新的识别城市绿地（UGS）社会功能的方法，结合高分辨率遥感影像与POI数据。方法：首先从三种数据（高分二号影像、POI和道路网）中提取5个信息图层，然后利用这些信息进行社会功能分类如图3所示。
    - **方法**：
        1. 预处理：利用HPEM方法自动提取城市植被，聚合POI类型，利用OSM道路网数据生成地块；
        2. 社会功能分类：邻近凸包分析法（NCHA）区分公园绿地和附属绿地，Text-concave-hull分析方法（TCHA）提取住宅相关的信息，利用ArcGIS软件识别缓冲区绿地。
- **2018 - Beyond Word2vec: An approach for urban functional region extraction and identification by combining Place2vec and POIs**
    - **内容**：介绍了一种通过整合POI数据和简化的Place2vec模型来检测邻域尺度(NA)功能区的方法。
    - **方法**：
        1. 首先采用最近邻法获取基于POI的空间上下文数据；
        2. 根据POI与中心POI之间的距离权重来增加POI对的数量；
        3. 利用skip-gram方法提取POI的高维特征向量；
        4. 在邻域尺度（NA）应用K-Means方法来聚类POI向量，得到功能区分类。
- **2019 - Exploring semantic elements for urban scene recognition: Deep integration of high-resolution imagery and OpenStreetMap (OSM)**
    - **内容**：本文结合OSM数据与高分辨率遥感影像实现城市场景识别。本文策略依次从像素、对象和场景角度对场景内容进行理解。具体而言，本文首先将OSM数据与高分辨率遥感影像融合，生成大量可用于深度学习框架训练的语义元素，然后从POI中提取高级语义用以丰富影像特征，最后计算语义对象的空间分布模式进行场景分类。
    - **方法**：
        1. 从OSM数据和遥感影像中提取语义元素；
        2. 利用CNN识别地物对象；
        3. 为了使地物能从功能语义方面更好地识别，引入POI数据;
        4. 利用空间测量评估城市空间属性，基于语义内容和空间属性，可以对城市场景进行分类。
- **2020 - Large-scale urban functional zone mapping by integrating remote sensing images and open social data**
    - **内容**：目前的利用遥感影像或社交媒体数据来研究城市功能区（UFZ）的方法侧重于在小范围内对功能区进行绘图，本文提出一种将遥感影像与社交媒体数据相结合的方法从大尺度上绘制城市功能区。
    - **方法**：
        1. 首先采用一种基于上下文的方法将影像与道路结合生成UFZ研究单元；
        2. 利用KMeans将从影像中提取的光谱特征以及两种景观指标（PLAND、AI）生成单词，同时将每个POI的类别视为单词；
        3. 利用LDA模型从中挖掘语义特征；
        4. 采用SVM分类器进行分类。