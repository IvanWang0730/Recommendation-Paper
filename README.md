# Recommendation-Paper

2023.2.7-周二
CTR论文-MEITUAN

1. 层次化Attention: Current Click Behavior > Click Behavior > Other Behavior
2. 对比学习解决稀疏性
模型去选择Key Points...? Behavior Adaptive Hierarchical Interest

Motivation:
1. Explicit decision-making context: the relation of the intra-page items
2. Implicit decision-making context: the information introduced by personalization
Model:
1. Irrelevance Suppression Unit (ISU): 过滤Explicit和Implicit context中不相关的items，MLP
2. Relevance Interaction Unit (RIU): Query为clicked item K,V为scope内的itmes cross-attention做选择
3. Adaptive Interest Aggregation Unit (AIAU): 类似DIN利用cross-attention对历史行为兴趣选择，单层Transfomer Decoder Layer
Datasets: Avito & MeituanAds

2023.2.8-周三
