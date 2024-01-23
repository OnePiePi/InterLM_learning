# LLM (large language model)

第一次课程视频链接：https://www.bilibili.com/video/BV1Rc411b7ns/

相比于专用模型，我们现在越来越对通用模型展现出更多的兴趣。

从模型到应用存在gap，我们常使用下面的流程图来完成这个跨越。

![image-20240113152527729](C:\Users\OnePie\AppData\Roaming\Typora\typora-user-images\image-20240113152527729.png)

书生·浦语 全链条开源开放体系

![image-20240117155335778](C:\Users\OnePie\AppData\Roaming\Typora\typora-user-images\image-20240117155335778.png)

1. 万卷 开源的多模态语料库 超过2TB大小（内容和主流价值观对齐？不太自由说实话）。

   可以到 opendatalab 这个平台去浏览和下载。

2. 预训练 多卡效率高 性能优化高 兼容 HUggingFace 开箱即用

   增量续训：学习新知识 有监督微调：学会理解和遵循各种指令

   高效的微调框架 XTuner 适配20系以上的所有显卡 现存优化较好 

3. 评测 OpenLLM Leaderboard 是 HuggingFace 这个机构提出的测试集

   我们的开源评测体系：OpenCompass

   ![image-20240117191710455](C:\Users\OnePie\AppData\Roaming\Typora\typora-user-images\image-20240117191710455.png)

4.  部署 LMDeploy

   面临的挑战：内存开销巨大，token逐个生成，数量不定，模型结构相对简单，像transformer结构大部分是decoder-only

   在小飞机设备上如何部署？如何加速推理，解决动态shape问题，如何有效管理和利用内存，提升系统整体吞吐量，降低请求的平均响应时间。

   LMDeploy可以提供模型轻量化的功能 4bit权重量化

   ![image-20240117210443013](C:\Users\OnePie\AppData\Roaming\Typora\typora-user-images\image-20240117210443013.png)

5. 大语言模型的局限性

   - 最新信息和知识的获取
   - 回复的可靠性
   - 数学计算
   - 工具使用和交互

   ![image-20240117210853704](C:\Users\OnePie\AppData\Roaming\Typora\typora-user-images\image-20240117210853704.png)

6. 智能体框架 Lagent

   ![image-20240117210951645](C:\Users\OnePie\AppData\Roaming\Typora\typora-user-images\image-20240117210951645.png)

   还有多模态智能体工具箱 AgentLego

   ![](https://raw.githubusercontent.com/OnePiePi/image_host@main/img/image-20240117212146963.png)



## 实践环节 

熟悉算力平台的使用，完成开发及创建及本地连接操作
