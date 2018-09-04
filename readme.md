1. 如何定义机器学习？机器学习是为了构建可根据数据学习的系统。学习意味着在某项任务中取得更好的成绩, 给出一些性能指标。
2. 机器学习可以解决的四类问题？机器学习很适合解决那些我们没有算法方案来解决的复杂问题，可以替换长时间的手动调整规则列表，构建适应波动环境的系统,，最后帮助人类学习（如：数据挖掘）。
3. 什么是带标签的训练集？一个训练集包含了每个实例所需的解决方案（也可理解为预期的结果）.
4. 最常见的两个监督任务是什么？回归和分类
5. 指出四个常见的非监督任务？聚类，可视化，降维，关联规则学习
6. 要让一个机器人能在各种未知地形行走，你会采用什么机器学习算法？强化学习可能会表现得最好，因为这通常是强化学习处理的问题类型。也许可以把这个问题表达为一个有监督或半监督的学习问题，但这将是不太自然的。
7. 要对你的顾客进行分组，你会采用哪类算法？如果你不知道如果定义分组，则可以通过聚类算法（无监督学习）将客户细分为类似客户的集群。但是，当你知道你想要哪些组，则可以将每个分组中的示例提供给分类算法中（监督学习），然后它会将你的顾客归类到这些群组中。
8. 垃圾邮件检测是监督学习问题，还是非监督学习问题？垃圾邮件检测是一个很经典的监督学习问题：该算法需要提供很多带有标签的邮件 (垃圾邮件或非垃圾邮件) 一起。
9. 什么是在线学习系统？一个在线学习系统可以逐步学习，而不是分批学习系统。这使得它能够快速适应不断变化的数据和自治系统， 以及对大量数据进行训练。
10. 什么是核外学习（out-of-core learning）？核外（out-of-core）算法可以处理大量无法容纳在计算机主内存中的数据。一个核外学习算法将数据分割成小数据块，并使用在线学习技术从这些小数据块中学习。
11. 什么学习算法是用相似度做预测？基于实例的学习系统通过心学训练数据。然后，当给定一个新实例时，它使用相似性度量来查找最相似的学习实例，并使用它们进行预测。
12. 模型参数和学习算法的超参数的区别是什么？模型有一个或多个模型参数来决定当定一个新实例将预测什么 (如：线性模型的斜率)。学习算法试图找到这些参数的最佳值，使模型能够很好地推广到新的实例。超参数是学习算法本身的参数，而不是模型 (如：应用的正则化量)。
13. 基于模型学习的算法搜寻的是什么？最成功的策略是什么？基于模型学习如何做预测？基于模型的学习算法搜索模型参数的最优值，使模型能够很好地推广到新实例。我们通常通过最小化成本函数来训练这样的系统，它能测量系统在对训练数据进行预测时的糟糕程度，再加上在模型正规化时对模型复杂度的惩罚。为了进行预测, 我们利用学习算法找到的参数值，将新实例的特征引入到模型的预测函数中。
14. 机器学习的四个主要挑战是什么？机器学习中的一些主要挑战是缺乏数据，数据质量不高，缺乏代表性，无特点，过于简单的模型欠拟合数据，以及过度复杂的模型过度拟合数据。
15. 如果模型在训练集上表现好，但推广到新实例表现差，问题是什么？给出三个可能的解决方案。这个模型可能过度拟合了训练数据（或者是我们得到了幸运的训练数据）。过度拟合可能的解决办法就是获取更多的数据，简化模型（选择更简单的算法，减少使用的参数或特征的数量，或使模型更加规范化），或对训练数据降噪。
16. 什么是测试集，为什么要使用它？模型在生产中启动之前，使用测试集来估计模型对新实例产生的泛化误差。
17. 验证集的目的是什么？验证集用于比较模型。它将使我们尽可能得选择最佳模型和优化超参数。
18. 如果用测试集调节超参数，会发生什么？如果你使用测试集来调节超参数，你冒着过度拟合测试集得风险，并且你度量的泛化误差将是乐观的 (你可能会启动一个性能比预期更差的模型)。
19. 什么是交叉验证，为什么它比验证集好？交叉验证是一项用来比较模型的技术 (用于模型选择和超参数优化)，而无需单独的验证集。这将节省宝贵的训练数据。