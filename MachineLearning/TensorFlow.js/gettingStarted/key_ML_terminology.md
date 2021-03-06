## 机器学习的主要术语

1. 标签：是指我们要预测的真实事物：y
    1. 基本线性回归中的 y 变量。可以是小麦未来的价格、图片中显示的动物品种、音频剪辑的含义或者任何事物。
2. 特征：是指用于描述数据的输入变量：x[i]
    1. 基本线性回归中的 {x1, x2, x3,…, xn} 变量。简单的机器学习项目可能会使用单个特征，而比较复杂的机器学习项目，可能会使用数百万个特征。
    2. 示例：如在垃圾邮件检测器中，特征可能包括：邮件中的字词、发件人的地址、发送邮件的时间段等等
3. 样本：是指数据的特定实例：**x** (粗体 x 表示它是一个矢量)
    1. 有标签样本具有 {特征，标签}: {x, y}
        1. 用于训练模型
    2. 无标签样本具有 {特征，？}: {x, ?}
        1. 用于对新数据做出预测
4. 模型：可将样本 x' 映射到预测标签：y’。重点：模型生命周期中的两个阶段
    1. 训练：是指创建或学习模型。也就是说，向模型逐渐学习特征与标签之间的关系。
    2. 推断：是指将训练后的模型应用于无标签样本，也就是说，使用经过训练的模型做出有用的预测。例如，对于输入[1,2,3,4]，输出[1,3,5,7]，模型在经过训练后，输入`10`可以预测输出是`18.99978348`，很接近答案`19`。
5. 回归与分类
    1. 回归模型：可预测连续值。例如：回归模型做出的预测可以回答如下问题
        1. 深圳一栋房产的价值是多少？
        2. 用户点击一个广告的概率是多少？
    2. 分类模型：可以预测离散值。例如，分类模型做出的预测可以回答如下问题
        1. 某个电子邮件是垃圾邮件还是非垃圾邮件
        2. 这是一张狗还是猫还是老虎的照片
