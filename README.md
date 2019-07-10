# bilstm + conv + mlp的神经网络模型

## 场景
    1. 处理query-pair的相似度问题, 输入文件每行格式为: query1\tquery2\tscore; 问题等价时score=1.0否则score=0.0

## 思路
    1. 输入层使用字符粒度的向量
    2. 隐藏层使用bilstm + conv(max-pooling)对query进行encoder
    3. 使用多层感知机计算输出

