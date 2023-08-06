# XunFeiCompetition-AIQuantitativeFinance
讯飞开放平台——AI量化模型预测挑战赛

## 赛事任务
**数据集：** 给定训练集（含验证集）， 包括10只（不公开）股票、79个交易日的L1snapshot数据（前64个交易日为训练数据，用于训练；后15个交易日为测试数据，不能用于训练）， 数据已进行规范化和隐藏处理，包括5档量/价，中间价，交易量等数据。  
__预测任务：__ 利用过往及当前数据预测未来中间价的移动方向，在数据上进行模型训练与预测  
__输入数据：__  
行情频率：3秒一个数据点（也称为1个tick的snapshot）；  
每个数据点包括当前最新成交价/五档量价/过去3秒内的成交金额等数据；  
训练集中每个数据点包含5个预测标签的标注； 允许利用过去不超过100tick（包含当前tick）的数据，预测未来N个tick后的中间价移动方向。  
预测时间跨度：5、10、20、40、60个tick，5个预测任务；  
即在t时刻，分别预测t+5tick，t+10tick，t+20tick，t+40tick，t+60tick以后： 最新中间价相较t时刻的中间价：下跌/不变/上涨。  
__评估指标__ 本模型依据提交的结果文件，采用macro-F1 score进行评价，取label_5, label_10, label_20, label_40, label_60五项中的最高分作为最终得分。本模型依据提交的结果文件，采用macro-F1 score进行评价，取label_5, label_10, label_20, label_40, label_60五项中的最高分作为最终得分。

## 方案
__1__ 数据EDA    
__2__ 特征工程    
__3__ 划分训练集、验证集和测试集    
__4__ 机器学习模型选择    
__5__ 模型训练    
__6__ 验证    
__7__ 调参    
__8__ 集成学习策略    
__9__ 测试  


