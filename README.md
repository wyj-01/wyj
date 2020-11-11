# wyj
       此次作业所选用的是“良/恶性乳腺癌肿瘤预测”的相关数据，并选取以下4种方法进行预测。
      # 1.决策树
       决策树算法是一种逼近离散函数值的方法。它是一种典型的分类方法，首先对数据进行处理，利用归纳算法生成可读的规则和决策树，然后使用决策对新数据进行分析。
       相比于其他学习模型,决策树在模型描述上有着巨大的优势。决策树的推断逻辑非常直观,具有清晰的可解释性，也方便了模型的可视化。这些特性同时也保证在使用决策树模型时，是无须考虑对数据的量化甚至标准化的。并且，与K近邻模型不同，决策树仍然属于有参数模型,需要花费更多的时间在训练数据上。
      # 2.线性分类器
       线性分类器是一种假设特征与分类结果存在线性关系的模型。这个模型通过累加计算每个维度的特征与各自权重的乘积来帮助类别决策。
      线性分类器可以说是最为基本和常用的机器学习模型。尽管其受限于数据特征与分类目标之间的线性假设，我们仍然可以在科学研究与工程实践中把线性分类器的表现性能作为基准。
      # 3.支持向量机
       支持向量机是一类按监督学习方式对数据进行二元分类的广义线性分类器，其决策边界是对学习样本求解的最大边距超平面。
       支持向量机模型曾经在机器学习研究领域繁荣发展了很长一段时间。主要原因在于其精妙的模型假设可以帮助我们在海量甚至高维度的数据中,筛选对预测任务最为有效的少数训练样本。这样做不仅节省了模型学习所需要的数据内存，同时也提高了模型的预测性能。然而，要获得如此的优势就必然要付出更多的计算代价。
      # 4.k近邻算法
       K近邻分类算法，是一个理论上比较成熟的方法，也是最简单的机器学习算法之一。该方法的思路是：在特征空间中，如果一个样本附近的k个最近(即特征空间中最邻近)样本的大多数属于某一个类别，则该样本也属于这个类别。
      该模型没有参数训练过程，因此k近邻属于无参数模型中非常简单的一种，但导致了其非常高的计算复杂度和内存消耗。
#实验过程

1.将数据导入，存储到data中;

2.去除有数据缺失的样本;

3.对数据进行划分，80%的样本作为训练集，20%的样本作为测试集;|

4.对数据进行预处理，保证数据的每个维度均值为0，方差为1;

5.分别用单一决策树， 逻辑斯蒂回归模型，随机梯度参数，支持向童机和k近邻算法进行训练和预测;

6.比较几种方法训练的准确率。

方法           单一决策树    逻辑斯蒂回归     随机梯度参数    支持向里机     k近邻算法

准确率           0.920             0.949                0.964               0.949            0.956

由上述数据可知，在“良/恶性乳腺癌肿瘤预测“的样本中，随机梯度参数的预测准确率最高，单一决策树的预测准 确率最低。
