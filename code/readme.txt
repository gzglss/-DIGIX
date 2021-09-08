数据预处理：
1.data_preprocess_divide_train.py#将原始训练集的有标签数据、无标签数据分开
2.data_preprocess_cleardata.py#清理文本中的html、空格以及body中与title重复的部分
3.data_preprocess_split_data.py#截取body的长度

多分类模型训练：
1.bert_transform_classification.py#用bert搭建模型一
2.bertwwm_transform_classification.py#用bertwwm搭建模型二
3.macbert_transform_classification.py#用macbert搭建模型三
4.Train_Bert_transform.py#训练bert
5.Train_Bert_transform_wwm.py#训练bertwwm
6.Train_Bert_transform_mac.py#训练macbert

二分类模型：
1.data_encode.py#给文本编码
2.binary_classificator.py#对抗训练二分类模型，预测测试集中的其他与非其他

预测：
1.test_predict.py

运行：
1.main.py #运行全部过程，包括数据处理、模型训练与预测，从头到尾运行
2.preprocess.py #运行数据预处理的部分
3.training.py #运行模型训练部分
4.predict.py #运行测试集预测部分