# Recommendation-Paper

### CTR论文-MEITUAN

#### [A Deep Behavior Path Matching Network for Click-Through Rate Prediction, WWW2023(short)](https://github.com/IvanWang0730/Recommendation-Paper/blob/main/A%20Deep%20Behavior%20Path%20Matching%20Network%20for%20Click-Through%20Rate%20Prediction.pdf)
1. Intuition:
* 层次化Attention: Current Click Behavior > Click Behavior > Other Behavior
* 对比学习解决稀疏性
2. 模型去选择Key Points...? Behavior Adaptive Hierarchical Interest

#### [Decision-Making Context Interaction Network for Click-Through Rate Prediction, AAAI2023](https://github.com/IvanWang0730/Recommendation-Paper/blob/main/Decision-Making%20Context%20Interaction%20Network%20for%20Click-Through%20Rate%20Prediction.pdf)
1. Motivation:
* Explicit decision-making context: the relation of the intra-page items
* Implicit decision-making context: the information introduced by personalization
2. Model:
* Irrelevance Suppression Unit (ISU): 过滤Explicit和Implicit context中不相关的items，MLP
* Relevance Interaction Unit (RIU): Query为clicked item K,V为scope内的itmes cross-attention做选择
* Adaptive Interest Aggregation Unit (AIAU): 类似DIN利用cross-attention对历史行为兴趣选择，单层Transfomer Decoder Layer
3. Datasets:
* Avito & MeituanAds

#### [Contrastive Learning for Sequential Recommendation, ICDE](https://github.com/IvanWang0730/Recommendation-Paper/blob/main/Contrastive%20Learning%20for%20Sequential%20Recommendation.pdf)
