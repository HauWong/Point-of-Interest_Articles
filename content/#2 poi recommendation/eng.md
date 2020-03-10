> 共11篇

- **2014 - Graph-based Point-of-interest Recommendation with Geographical and Temporal Influence**
    - **内容**：研究发现：(1)用户倾向于访问附近的地方，(2)用户倾向于在不同的时间段访问不同的地方，而在同一时间段，用户倾向于定期访问相同的地方。本文重点讨论了基于时间感知的POI推荐问题，其目的是为用户推荐一个在特定时间访问的POI列表。本文提出了基于广度优先的偏好传播算法，通过构建地理空间影响感知图（Geographical-Temporal influences Aware Graph，GTAG）实现签到记录、地理影响和时间影响之间建模。
- **2016 - Effective successive POI recommendation inferred with individual behavior and group preference**
    - **内容**：利用用户行为与偏好能够实现个性化的位置服务，比如POI推荐，但每个用户的可用数据非常少，且用户数量大，计算复杂度高，因此实现精确的POI推荐具有较大挑战性。本文提出一种基于类别与分组的个性化连续POI推荐方法。
    - **方法**：
        1. 基于居住位置和位置类别的个偏好对用户进行分组；
        2. 基于分组进行类别推荐；
        3. 基于类别进行位置推荐。
- **2016 - POI Recommendation: A Temporal Matching between POI Popularity and User Regularity**
    - **内容**：与传统的以兴趣为导向的商品推荐不同，POI因受时间的影响，其推荐应用更加复杂。先前的研究将时间影响考虑到POI推荐中，但却忽略了POI的流行度随时间的变化以及一些用户的限制。本文提出一种将用户与POI之间在时间上的匹配度加入POI推荐应用中。
    - **方法**：
        1. 首先通过挖掘POI类别和人类活动的时空规律，对POI流行度随时间的变化进行分析；
        2. 通过一个用户-POI匹配函数，学习一种用户规则来描述用户定期访问POI的规律。
- **2017 - A temporal-aware POI recommendation system using context-aware tensor decomposition and weighted HITS**
    - **内容**：对于传统的基于协同过滤的POI推荐方法来说，用户位置矩阵非常稀疏，并且时间影响在POI推荐中也起着重要作用，考虑当上述问题，本文提出一种新型POI推荐系统，该系统由两部分组成：针对用户偏好建模的情景感知张量分解（CTD）、基于加权HITS（Hypertext Induced Topic Search）的POI排名（WHBPR）。
    - **方法**：本文从三个维度（用户、类型和时间）对用户的偏好进行建模得到一个三维张量，CTD算法利用三个矩阵来补充用户偏好张量的缺失项，以恢复用户对不同时间段的偏好，WHBPR整合了用户偏好和社会观点对POI排名的影响。

- **2017 - CTF-ARA: An adaptive method for POI recommendation based on check-in and temporal features**
    - **内容**：现存的很多POI推荐方法没有考虑到签到数据多样性特征的影响，本文提出一种将签到数据和时间特征与基于用户的协同过滤相结合的自适应POI推荐方法（CTF-ARA）
    - **方法**：
        1. 使用概率统计分析挖掘用户活动和签到行为的相似特征，以及时间因素的多样性和连续性特征；
        2. 利用K-Means方法将用户分为活跃用户和非活跃用户，并基于所提取的特征设计了一个相似用户过滤算法；
        3. 最后利用不同时间段的余弦相似度平滑技术实现POI推荐，该算法能根据用户的活动自适应调整。
- **2019 - Using POI functionality and accessibility levels for delivering personalized tourism recommendations**
    - **内容**：本文提出一种基于用户和兴趣点的旅游推荐系统，该系统综合考虑了用户的生理和心理限制，此外本文也提出一种考虑POI可达性的POI分类方法。
    - **方法**：
        1. 知识层：从多个维度的知识（机体功能、印象、情感、标签和社会模型）来表示用户，从多个维度（可达性、印象和标签）表示POI；
        2. 推理层：设计规则综合考虑知识层中的各个维度，推荐POI；
        3. 原型层：实现算法，验证输出。
- **2019 - Real-time event embedding for POI recommendation**
    - **内容**：本文提出一种实时POI嵌入模型，用以实现更合理的POI推荐应用。该方法的亮点在于能够从具有地理标签的推文中挖掘实时信息，学习隐含表达。
    - **方法**：
        1. 数据预处理：推文过滤和POI过滤；
        2. 事件与POI嵌入：一种实时POI嵌入算法，该算法即考虑了事件嵌如的实时信息，又考虑了嵌入的内在信息，分为两步：POI实例嵌、POI固有嵌入；
        3. 实时POI推荐系统：将推荐模型简化为一个二分类问题，预测用户在特定时间内是否对POI感兴趣。
- **2019 - Exploiting Geographical-Temporal Awareness Attention for Next Point-of-Interest Recommendation**
    - **内容**：现存的方法忽略了用户签到的过程，无法捕获在整个签到历史中POI与POI之间的关系。为解决该问题，本文提出一种地理-时间感知的多层注意力模型（GT-HAN）。
    - **方法**：
        1. 嵌入层：将POI映射到另一个语义空间，即对于每一个POI，将创建对应的POI偏好向量、地理影响向量和地理敏感（geo-susceptibility）向量，其中地理影响向量表达用户从该POI访问其他POI的趋势，地理敏感向量则表达POI接受来自其他POI用户的访问趋势，最终结合特征矩阵生成各向量对应的矩阵；
        2. 地理-时间注意力网络：建立地理关系→建立序列依赖
        3. Co-Attention网络：采用一种隐含的融合策略来连接加权注意力值和非线性连接层来学习动态用户偏好；
        4. 模型学习与优化。
- **2020 - Heterogeneous graph-based joint representation learning for users and POIs in location-based social network**
    - **内容**：由于（Location-based social network）LBSN中的一些上下文因子（地理影响、用户社会关系及时间信息等）之间存在异质性，很难从其中学习隐含表达。本文针对LBSN中的用户和POI提出一种新的联合表达学习框架（UP2VEC），构建一种异构图来整合上述因子。并进行了POI推荐和社交链接预测实验。
    - **方法**：
        1. LBSN图架构：首先对LBSN数据进行分析（签到频率、地理影响以及时序影响分析），再结合用户和POI构建图，计算节点间的迁移概率，最后利用Node2Vec从LBSN图上的用户和POI中学习隐含表达。
        2. 利用节点样本进行表达学习。
- **2020 - GLR: A graph-based latent representation model for successive POI recommendation**
    - **内容**：传统的POI推荐与连续POI推荐的区别在于，连续的POI推荐侧重于向用户推荐在一段时间内访问的POI。本文提出一种基于图的隐含表达模型（Graph-based Latent Representation，GLR），该模型基于历史签到数据获取时序变化影响（temporal successive transition influence）和用户偏好的隐含向量，提出一种GLR_GT方法利用隐含向量和POI的地理影响实现连续POI推荐。此外，本文提出一种结合LSTM的扩展方法GLR_GT_LSTM，用以模拟用户迁移行为。
    - **方法**：
        1. 基于图的隐含表达模型（GLR）
            1. 采用一种类别-频率树的模型将POI类别和签到数据嵌入隐含向量，并利用POI隐含向量构建所有区域的隐含向量；
            2. 利用GLR和获得的隐含向量分别从POI和区域的角度构建时序变化影响（temporal successive transition influence）和用户动态偏好的隐含向量。
            3. 最后，将这些隐含向量整合为用户意愿向量。
        2. 连续POI推荐方法
            1. 采用GLR_GT方法利用从POI和区域角度的时序变化影响和用户偏好以及地理影响来实现连续的POI推荐；
            2. GLR_GT_LSTM方法采用LSTM对用户复杂的连续迁移行为进行建模。
- **2020 - Modeling hierarchical category transition for next POI recommendation with uncertain check-ins**
    - **内容**：用户常常会留下一些无法精确到单个POI的签到信息，这些签到信息往往出现在一个POI集合中，然而在签到信息不准确的情况下，很难学习到准确的用户迁移模式，同时也加剧了冷启动的问题。为此，本文设计了一种多层类别变化框架（HCT），利用不同层次的类别变化在不同粒度上发现用户的偏好迁移模式。