# 数据库系统论文翻译与学习

> 建立这个仓库的初衷是记录自己学习分布式系统、数据库系统、机器学习、大数据等一些有意思的事情。

如何使用？

* 论文的标题链接到原文，在已经翻译完成的论文标题前面会有一个椰子树。点击标题后方的查看翻译链接会打开对应的页面。
* 这些页面使用Markdown编写，每个Markdown文件会对应一个与文件相同的目录用于存放一些资源文件，例如图片等。

# 目录

## CMU 15-721 高级数据库系统 春季 2020

* 数据库课程介绍与数据库历史
	* [M. Stonebraker, et al., 数据库系统阅读中的"有来有往", 第四版, 2006 (可选的)]()
	* [A. Pavlo, et al., NewSQL有什么新功能?, in SIGMOD Record (vol. 45, iss. 2), 2016 (可选的)]()

* 内存数据库
	* [X. Yu, et al., 凝视深渊: 千核并发控制的评估, in VLDB, 2014]()
	* [S. Harizopoulos, et al., 透过镜子看OLTP，我们在那里发现了什么, in SIGMOD, 2008 (可选的)]()
	* [H. Garcia-Molina, et al., 主存数据库系统综述, in IEEE Trans. on Knowl. and Data Eng., 1992 (可选的)]()

* 多版本并发控制 (设计决策)
	* [Y. Wu, et al., 内存中多版本并发控制的实证评估, in VLDB, 2017]()
	* [D.R.K. Ports, et al., PostgreSQL中的可序列化快照隔离, in VLDB, 2012 (可选的)]()
	* [Y. Huang, et al., 竞争的主存多核事务中的乐观机会, in VLDB, 2020 (可选的)]()

* 多版本并发控制 (协议)
	* [T. Neumann, et al., 主存数据库系统的快速可串行化多版本并发控制, in SIGMOD, 2015]()
	* [H. Lim, et al., Cicada:可靠快速的多核内存事务, in SIGMOD, 2017 (可选的)]()
	* [P.-A. Larson, et al., 主存数据库的高性能并发控制机制, in VLDB, 2011 (可选的)]()

* 多版本并发控制 (垃圾回收)
	* [J. Böttcher, et al., 内存中MVCC系统的可扩展垃圾收集, in VLDB, 2019]()
	* [J. Lee, et al., 面向多版本并发控制的混合垃圾收集, in SIGMOD, 2016 (可选的)]()

* OLTP 索引 (B+树 数据结构)
	* [Z. Wang, et al., 构建一棵Bw树需要的不仅仅是流行语, in SIGMOD, 2018]()
	* [S.K. Cha, et al., 共享内存多处理器系统中主存索引的缓存感知并发控制, in VLDB, 2001 (可选的)]()
	* [G. Graefe, B树锁定技术综述, in TODS, 2010 (可选的)]()
	* [J. Levandoski, et al., B树:新型硬件的B树, in ICDE, 2013 (可选的)]()
	* [J. Faleiro, et al., 数据库系统中的无锁同步: 银弹还是黄金?, in CIDR, 2017 (可选的)]()
	* [T. Kissinger, et al., KISS树: 现代架构上的智能无闩锁内存索引, in DaMoN, 2012 (可选的)]()

* OLTP 索引 (Trie 数据结构)
	* [V. Alvarez, et al., 自适应基数树和哈希表的比较, in ICDE, 2015 ]()
	* [V. Leis, et al., 自适应基数树:内存数据库的巧妙索引, in ICDE, 2013 (可选的)]()
	* [V. Leis, et al., 实用同步的艺术, in DaMoN, 2016 (可选的)]()
	* [R. Binna, et al., 热: 内存数据库系统的高度优化索引, in SIGMOD, 2018 (可选的)]()

* 存储模型, 数据布局和系统目录
	* [M. Athanassoulis, et al., 混合工作负载的最佳列布局, in VLDB, 2019 ]()
	* [J. Arulraj, et al., 连接混合工作负载的行存储和列存储, in SIGMOD, 2016 (可选的)]()
	* [I. Alagiannis, et al., H2O: 免提自适应商店, in SIGMOD, 2014 (可选的)]()
	* [M. Grund, et al., HYRISE: 主存储器混合存储引擎, in VLDB, 2010 (可选的)]()
	* [D. Abadi, et al., 列存储与行存储: 他们真的有多不同?, in SIGMOD, 2008 (可选的)]()

* 数据库压缩
	* [D. Abadi, et al., 在面向列的数据库系统中集成压缩和执行, in SIGMOD, 2006 ]()
	* [C. Binnig, et al., 基于字典的主存列存储保序字符串压缩, in SIGMOD, 2009 (可选的)]()
	* [I. Müller, et al., 内存列存储数据库系统中的自适应字符串字典压缩, in EDBT, 2014 (可选的)]()
	* [V. Raman, et al., 如何拧干表:关系的熵压缩和压缩关系的查询, in VLDB, 2006 (可选的)]()
	* [H. Zhang, et al., 用混合索引降低主存OLTP数据库的存储开销, in SIGMOD, 2016 (可选的)]()
	* [C. Liu, et al., 大多是保序词典, in ICDE, 2019 (可选的)]()

* 恢复协议
	* [P. Antonopoulos, et al., Azure数据库中的常数时间恢复, in VLDB, 2019 ]()
	* [W. Zheng, et al., 通过多核并行实现快速持久性和恢复的快速数据库, in OSDI, 2014 (可选的)]()
	* [A. Goel, et al., 在Facebook快速重启数据库, in SIGMOD, 2014 (可选的)]()
	* [K. Ren, et al., 主存数据库系统中的低开销异步检查点, in SIGMOD, 2016 (可选的)]()
	* [N. Malviya, et al., 对主存OLTP恢复的再思考, in ICDE, 2014 (可选的)]()

* 网络协议
	* [M. Raasveldt, et al., 不要劫持我的数据:客户端协议重新设计案例, in VLDB, 2017 ]()
	* [F. Li, et al., 利用远程内存和RDMA加速关系数据库, in SIGMOD, 2016 (可选的)]()
	* [F. Binnig, et al., 慢速网络的终结:是时候重新设计了, in VLDB, 2016 (可选的)]()

* 调度
	* [V. Leis, et al., Morsel驱动的并行性:一个面向众核时代的NUMA感知查询评估框架, in SIGMOD, 2014 ]()
	* [I. Psaroudakis, et al., 扩大并发主内存列存储扫描:实现自适应NUMA感知数据和任务布局, in VLDB, 2015 (可选的)]()
	* [I. Psaroudakis, et al., 面向高并发分析和事务性主存工作负载的任务调度               , in ADMS, 2013 (可选的)]()
	* [D. Porobic, et al., 硬件孤岛上的OLTP, in VLDB, 2012 (可选的)]()

* 查询执行和处理
	* [M. Kester, et al., 主存优化数据系统中的访问路径选择:我应该扫描还是应该探测?, in SIGMOD, 2017 ]()
	* [P. Boncz, et al., MonetDB/X100: 超流水线查询执行, in CIDR, 2005 (可选的)]()
	* [L. Shrinivas, et al., 垂直分析数据库中的物化策略:经验教训, in ICDE, 2013 (可选的)]()
	* [A. Mishra, et al., 使用动态内存表达式加速分析, in VLDB, 2016 (可选的)]()

* 查询编译
	* [T. Neumann, 高效编译现代硬件的高效查询计划, in VLDB, 2011 ]()
	* [K. Krikellas, et al., 生成用于整体查询评估的代码, in ICDE, 2010 (可选的)]()
	* [H. Pirk, et al., 内存驻留数据库的中央处理器和高速缓存高效管理, in ICDE, 2013 (可选的)]()
	* [B. Raducanu, et al.,矢量方向的微适应性, in SIGMOD, 2013 (可选的)]()
	* [A. Shaikhha, et al., 如何设计查询编译器, in SIGMOD, 2016 (可选的)]()
	* [A. Kohn, et al., 编译查询的自适应执行, in ICDE, 2018 (可选的)]()

* 矢量化执行
	* [O. Polychroniou, et al., 内存数据库SIMD矢量化的再思考, in SIGMOD, 2015 ]()
	* [T. Thomas Willhalm, et al., SIMD扫描:使用片内矢量处理单元的超快速内存表扫描, in VLDB, 2009 (可选的)]()
	* [Y. Li, et al., 位编织:主存数据处理的快速扫描, in SIGMOD, 2013 (可选的)]()

* 矢量化与编译
	* [T. Kersten, et al., 关于编译和矢量化查询，您一直想知道但又不敢问的一切, in VLDB, 2018 ]()
	* [P. Menon, et al., 内存数据库的松弛算子融合:最终使编译、矢量化和预取协同工作, in VLDB, 2017 (可选的)]()
	* [J. Sompolski, et al., 查询执行中的矢量化与编译, in DaMoN, 2011 (可选的)]()
	* [H. Lang, et al., 数据块:使用矢量化和编译的压缩存储上的混合OLTP和OLAP, in SIGMOD, 2016 (可选的)]()

* 并行联合算法 (Hash))
	* [S. Schuh, et al., 内存中十三个关系等连接的实验比较, in SIGMOD, 2016 ]()
	* [S. Richter, et al., 哈希方法的七维分析及其对查询处理的启示, in VLDB, 2015 (可选的)]()
	* [S. Blanas, et al., 多核处理器主存散列连接算法的设计与评估, in SIGMOD, 2011 (可选的)]()
	* [C. Balkesen, et al., 多核处理器上的主存散列连接:调整到底层硬件, in ICDE, 2013 (可选的)]()

* 并行联合算法 (排序)
	* [C. Balkesen, et al., 多核主内存连接:排序与散列的再探讨, in VLDB, 2013 ]()
	* [C. Kim, et al., 重新审视排序与散列:现代多核处理器上的快速连接实现, in VLDB, 2009 (可选的)]()
	* [G. Graefe, et al., 重新审视排序和散列, in TKDE, 1994 (可选的)]()
	* [M.-C. Albutiu, et al., 主存多核数据库系统中的大规模并行排序合并连接, in VLDB, 2012 (可选的)]()

* 优化器实现 (概览)
	* [S. Chaudhuri, 关系系统中的查询优化综述, in PODS, 1998 ]()
	* [G. Graefe, et al., 火山优化生成器:可扩展性和高效搜索, in ICDE, 1993 (可选的)]()
	* [G. Graefe, 查询优化的级联框架, in IEEE Data Engineering Bulletin, 1995 (可选的)]()
	* [M.A. Soliman, et al., Orca:面向大数据的模块化查询优化器架构, in SIGMOD, 2014 (可选的)]()
	* [L.D. Shapiro, et al., 在自顶向下查询优化中利用上下限, in IDEAS, 2001 (可选的)]()

* 优化器实现 (自上而下与自下而上)
	* [Yongwen Xu, 哥伦比亚数据库查询优化器的效率 (1-35页), in Portland State University, 1998 ]()
	* [J. Chen, et al., 内存SQL查询优化器, in VLDB, 2017 (可选的)]()
	* [G. Moerkotte, et al., 动态规划反击, in SIGMOD, 2008 (可选的)]()
	* [T. Neumann, et al., 连接的完整故事(在HyPer), in BTW, 2017 (可选的)]()
	* [E. Begoli, et al., Apache Calcite: 异构数据源上优化查询处理的基础框架, in SIGMOD, 2018 (可选的)]()

* 优化器实现 (替代方法)
	* [B. Ding, et al., 计划缝合:利用许多计划中最好的, in VLDB, 2018 ]()
	* [S. Babu, et al., 窥镜中的自适应查询处理, in CIDR, 2015 (可选的)]()
	* [J. Zhu, et al., 展望未来让查询计划变得强大, in VLDB, 2017 (可选的)]()
	* [R. Marcus, et al., Neo:一种学习型查询优化器, in VLDB, 2019 (可选的)]()
	* [I. Trummer, et al., SkinnerDB: 基于强化学习的后悔有界查询评估, in SIGMOD, 2019 (可选的)]()

* 代价模型
	* [V. Leis, et al., 查询优化器到底有多好?, in VLDB, 2015 ]()
	* [M. Stillger, et al., LEO - DB2的学习优化器, in VLDB, 2001 (可选的)]()
	* [Z. Yang, et al., 深度无监督基数估计, in VLDB, 2019 (可选的)]()
	* [J. Sun, et al., 基于端到端学习的成本估算器, in VLDB, 2019 (可选的)]()
	* [D. Vengerov, et al., 根据筛选条件估计连接大小, in VLDB, 2015 (可选的)]()
	* [Y. Chen, et al., 用于连接大小估计的两级抽样, in SIGMOD, 2017 (可选的)]()

* 大于内存的数据库
	* [V. Leis, et al., LeanStore: 主存之外的内存数据管理, in ICDE, 2018 ]()
	* [J. DeBrabant, et al., Anti-Caching: 数据库管理系统体系结构的新方法, in VLDB, 2013 (可选的)]()
	* [R. Stoica, et al., 为主存OLTP数据库启用高效的操作系统分页, in DaMoN, 2013 (可选的)]()
	* [G. Graefe, et al., 大数据的内存性能, in VLDB, 2014 (可选的)]()
	* [L. Ma, et al., 内存中OLTP数据库系统现代存储硬件上的大内存数据管理, in DaMoN, 2016 (可选的)]()

* 服务器端逻辑执行
	* [K. Ramachandra, et al., Froid: 关系数据库中命令程序的优化, in VLDB, 2017 ]()
	* [C. Duta, et al., 编译PL/SQL离开, in CIDR, 2020 (可选的)]()

* 新型硬件上的数据库
	* [J. Arulraj, et al., 写后日志记录, in VLDB, 2016 ]()
	* [M. Owaida, et al., Centaur: 一种混合式中央处理器-现场可编程门阵列数据库框架, in FCCM, 2017 (可选的)]()
	* [H. Kimura, FOEDUS: 面向千核和非易失性内存的OLTP引擎, in SIGMOD, 2015 (可选的)]()
	* [J. Power, et al., 图形处理器成为分析处理的主流, in DaMoN, 2015 (可选的)]()

## MIT 6.824 分布式系统

* [MapReduce:大型集群上的简化数据处理](./mit_6_824_分布式系统/mapreduce.pdf)
* [比特币:一种点对点的电子现金系统](./mit_6_824_分布式系统/bitcoin.pdf)
* [BlockStack:一个由区块链保护的全球命名和存储系统](./mit_6_824_分布式系统/blockstack-atc16.pdf)
* [支持高吞吐量和可用性的链复制](./mit_6_824_分布式系统/cr-osdi04.pdf/cr-osdi04.pdf)
* [不妥协:具有一致性、可用性和性能的分布式事务](./mit_6_824_分布式系统/farm-2015.pdf)
* [Google文件系统](./mit_6_824_分布式系统/gfs.pdf)
* [使用分布式、可扩展、方法化文件系统的体验:AnalogicFS](./mit_6_824_分布式系统/katabi-analogicfs.pdf)
* [安全不可信数据存储库](./mit_6_824_分布式系统/li-sundr.pdf)
* [寻找可理解的共识算法(扩展版)](./mit_6_824_分布式系统/raft-extended.pdf)
* [Spanner:Google的全球分布式数据库](./mit_6_824_分布式系统/spanner.pdf)
* [Frangipani:一个可扩展的分布式文件系统](./mit_6_824_分布式系统/thekkath-frangipani.pdf)
* [一个实用的容错虚拟机系统的设计](./mit_6_824_分布式系统/vm-ft.pdf)
* [弹性分布式数据集:内存集群计算的容错抽象](./mit_6_824_分布式系统/zaharia-spark.pdf)
* [Zookeeper:互联网规模系统的无等待协调](./mit_6_824_分布式系统/zookeeper.pdf)
* [在Faceboot的扩展内存缓存](./mit_6_824_分布式系统/memcache-fb.pdf)

## 数据库系统研发必备

* 本地引擎
	* [一个镜像损坏的案例](./数据库系统研发必备/本地引擎/A_Case_For_Fractured_Mirrors.pdf)
	* [非易失性存储器的OLTP数据库系统导论](./数据库系统研发必备/本地引擎/A_Prolegomenon_on_OLTP_Database_Systems_for_Non-Volatile_Memory.pdf)
	* [Anna:_适用于任何规模的键值存储](./数据库系统研发必备/本地引擎/Anna-_A_KVS_For_Any_Scale.pdf)
	* [Berleley_DB_Java版本架构](./数据库系统研发必备/本地引擎/Berkeley_DB_Java_Edition_Architecture.pdf)
	* [BzTree:_用于非易失性存储器的高性能无锁存范围索引](./数据库系统研发必备/本地引擎/BzTree-_A_High-Performance_Latch-free_Range_Index_for_Non-Volatile_Memory.pdf)
	* [面向快速多核键值存储的缓存技术](./数据库系统研发必备/本地引擎/Cache_Craftiness_for_Fast_Multicore_Key-Value_Storage.pdf)
	* [缓存无关的流式B树](./数据库系统研发必备/本地引擎/Cache-Oblivious_Streaming_B-trees.pdf)
	* [列存储与行存储,它们到底有多大区别](./数据库系统研发必备/本地引擎/Column-Stores_vs._Row-Stores-_How_Different_Are_They_Really.pdf)
	* [面向多核键值存储的并发日志结构内存](./数据库系统研发必备/本地引擎/Concurrent_Log-Structured_Memory_for_Many-Core_Key-Value_Stores.pdf)
	* [Data_Blocks:_使用矢量化和编译的压缩存储上的混合OLTP和OLAP](./数据库系统研发必备/本地引擎/Data_Blocks-_Hybrid_OLTP_and_OLAP_on_Compressed_Storage_using_both_Vectorization_and_Compilation.pdf)
	* [通过RDMA和缓存实现高效的分布式内存管理](./数据库系统研发必备/本地引擎/Efficient_Distributed_Memory_Management_with_RDMA_and_Caching.pdf)
	* [在键值存储上快速扫描](./数据库系统研发必备/本地引擎/Fast_Scans_on_Key-Value_Stores.pdf)
	* [探讨在非易失性存储器数据库系统上的存储和恢复方法](./数据库系统研发必备/本地引擎/Lets_Talk_About_Storage_&_Recovery_Methods_for_Non-Volatile_Memory_Database_Systems.pdf)
	* [现代B树技术](./数据库系统研发必备/本地引擎/Modern_B-Tree_Techniques.pdf)
	* [Tell:_面向混合负载的弹性数据库系统](./数据库系统研发必备/本地引擎/Tell-_An_Elastic_Database_System_for_Mixed_Workloads.pdf)
	* [编织关系以提高缓存性能](./数据库系统研发必备/本地引擎/Weaving_Relations_for_Cache_Performance.pdf)

* 共识与复制
	* [一个简单的全有序广播协议](./数据库系统研发必备/共识与复制/A_simple_totally_ordered_broadcast_protocol.pdf)
	* [读取MySQL二进制日志的API](./数据库系统研发必备/共识与复制/An_API_for_Reading_the_MySQL_Binary_Log.pdf)
	* [共识:_桥梁理论与实践](./数据库系统研发必备/共识与复制/Consensus-_Bridging_Theory_and_Practice.pdf)
	* [快速的Paxos](./数据库系统研发必备/共识与复制/Fast_Paxos.pdf)
	* [分布式迭代数据流的容错](./数据库系统研发必备/共识与复制/Fault-Tolerance_for_Distributed_Iterative_Dataflows_in_Action.pdf)
	* [普遍共识与Paxos](./数据库系统研发必备/共识与复制/Generalized_Consensus_and_Paxos.pdf)
	* [HT_Paxos:_大型集群数据中心的高吞吐量状态机复制协议](./数据库系统研发必备/共识与复制/HT-Paxos-_High_Throughput_State-Machine_Replication_Protocol_for_Large_Clustered_Data_Centers.pdf)
	* [寻找一个可理解的共识算法](./数据库系统研发必备/共识与复制/In_Search_of_an_Understandable_Consensus_Algorithm.pdf)
	* [可线性化:_并发对象的正确性条件](./数据库系统研发必备/共识与复制/Linearizability-_A_Correctness_Condition_for_Concurrent_Objects_.pdf)
	* [Ouroboros:_一个可证明安全的赌注证明区块链协议](./数据库系统研发必备/共识与复制/Ouroboros-_A_Provably_Secure_Proof-of-Stake_Blockchain_Protocol.pdf)
	* [Paxos现场制作:_工程视角](./数据库系统研发必备/共识与复制/Paxos_Made_Live_-_An_Engineering_Perspective.pdf)
	* [简单的Paxos](./数据库系统研发必备/共识与复制/Paxos_Made_Simple.pdf)
	* [实用的拜占庭容错和主动恢复](./数据库系统研发必备/共识与复制/Practical_Byzantine_Fault_Tolerance_and_Proactive_Recovery.pdf)
	* [SQL语句日志记录让SQLite真正变得精简](./数据库系统研发必备/共识与复制/SQL_Statement_Logging_for_Making_SQLite_Truly_Lite.pdf)
	* [多内核的可扩展数据库日志记录](./数据库系统研发必备/共识与复制/Scalable_Database_Logging_for_Multicores.pdf)
	* [松散耦合分布式系统的Chubby锁服务](./数据库系统研发必备/共识与复制/The_Chubby_lock_service_for_loosely-coupled_distributed_systems.pdf)
	* [一个兼职会议](./数据库系统研发必备/共识与复制/The_Part-Time_Parliament.pdf)
	* [分布式系统中的时间、时钟和事件排序](./数据库系统研发必备/共识与复制/Time,_Clocks,_and_the_Ordering_of_Events_in_a_Distributed_System.pdf)
	* [重新审视带视图标记的复制](./数据库系统研发必备/共识与复制/Viewstamped_Replication_Revisited.pdf)

* OLTP
	* [对ANSI_SQL隔离级别的评论](./数据库系统研发必备/OLTP/A_Critique_of_ANSI_SQL_Isolation_Levels.pdf)
	* [因果一致性和潜伏最优性:_朋友还是敌人](./数据库系统研发必备/OLTP/Causal_Consistency_and_Latency_Optimality-_Friend_or_Foe.pdf)
	* [分布式数据库系统中的并发控制](./数据库系统研发必备/OLTP/Concurrency_Control_in_Distributed_Database_Systems.pdf)
	* [共享数据库中锁的粒度和一致性程度](./数据库系统研发必备/OLTP/Granularity_of_Locks_and_Degrees_of_Consistency_in_a_Shared_Data_Base.pdf)
	* [主存数据库的高性能并发控制机制](./数据库系统研发必备/OLTP/High-Performance_Concurrency_Control_Mechanisms_for_Main_Memory_Databases.pdf)
	* [Omid,_重载:_可扩展和高可用的事务处理](./数据库系统研发必备/OLTP/Omid,_Reloaded-_Scalable_and_Highly-Available_Transaction_Processing.pdf)
	* [并发控制的乐观方法](./数据库系统研发必备/OLTP/On_Optimistic_Methods_for_Concurrency_Control.pdf)
	* [Spanner:_Google的全球分布式数据库](./数据库系统研发必备/OLTP/Spanner-_Google’s_Globally-Distributed_Database.pdf)
	* [技术报告:_高时钟不确定性的混合时间可访问的全球一致性](./数据库系统研发必备/OLTP/Technical_Report-_HybridTime_-_Accessible_Global_Consistency_with_High_Clock_Uncertainty.pdf)
	* [TicToc:_时间旅行乐观并发控制](./数据库系统研发必备/OLTP/TicToc-_Time_Traveling_Optimistic_Concurrency_Control.pdf)

* OLAP
	* [用于快速图形处理的分布式多GPU系统](./数据库系统研发必备/OLTP/A_Distributed_Multi-GPU_System_for_Fast_Graph_Processing.pdf)
	* [在GPU上加速动态图形分析](./数据库系统研发必备/OLTP/Accelerating_Dynamic_Graph_Analytics_on_GPUs.pdf)
	* [一种高效且符合语法习惯的流和表管理方法](./数据库系统研发必备/OLTP/An_Efficient_and_Syntactically_Idiomatic_Approach_to_Management_of_Streams_and_Tables.pdf)
	* [关系系统中查询优化综述](./数据库系统研发必备/OLTP/An_Overview_of_Query_Optimization_in_Relational_Systems.pdf)
	* [近似字符串处理](./数据库系统研发必备/OLTP/Approximate_String_Processing.pdf)
	* [BCC:_降低内存数据库乐观并发控制中的错误中止](./数据库系统研发必备/OLTP/BCC-_Reducing_False_Aborts_in_Optimistic_Concurrency_Control_with_Low_Cost_for_In-Memory_Databases.pdf)
	* [C_Store:_面向列的数据库管理系统](./数据库系统研发必备/OLTP/C-Store-_A_Column-oriented_DBMS.pdf)
	* [为IBM_Streams构建高效的Apache_Beam_Runner的挑战和经验](./数据库系统研发必备/OLTP/Challenges_and_Experiences_in_Building_an_Efficient_Apache_Beam_Runner_For_IBM_Streams.pdf)
	* [评估Weld中数据分析应用的端到端优化](./数据库系统研发必备/OLTP/Evaluating_End-to-End_Optimization_for_Data_Analytics_Applications_in_Weld.pdf)
	* [F1_Query:_大规模声明式查询](./数据库系统研发必备/OLTP/F1_Query-_Declarative_Querying_at_Scale.pdf)
	* [Gorilla:_一个快速、可伸缩的内存时序数据库](./数据库系统研发必备/OLTP/Gorilla-_A_Fast,_Scalable,_In-Memory_Time_Series_Database.pdf)
	* [图数据模型,_查询语言和编程范式](./数据库系统研发必备/OLTP/Graph_Data_Models,_Query_Languages_and_Programming_Paradigms.pdf)
	* [现代空间分析系统有多好](./数据库系统研发必备/OLTP/How_Good_Are_Modern_Spatial_Analytics_Systems.pdf)
	* [Mesa:_地理复制、近实时、可扩展的数据仓库](./数据库系统研发必备/OLTP/Mesa-_Geo-Replicated,_Near_Real-Time,_Scalable_Data_Warehousing.pdf)
	* [MonetDB_X100:_超级流水线查询执行](./数据库系统研发必备/OLTP/MonetDB_X100-_Hyper-Pipelining_Query_Execution.pdf)
	* [在Facebook提供串流加入服务](./数据库系统研发必备/OLTP/Providing_Streaming_Joins_as_a_Service_at_Facebook.pdf)
	* [大型数据库的查询评估技术](./数据库系统研发必备/OLTP/Query_Evaluation_Techniques_for_Large_Databases.pdf)
	* [内存数据库的宽松操作符融合——使编译、向量化和预取最终一起工作](./数据库系统研发必备/OLTP/Relaxed_Operator_Fusion_for_In-Memory_Databases-_Making_Compilation,_Vectorization,_and_Prefetching_Work_Together_At_Last.pdf)
	* [多核内存数据库中的快速事务](./数据库系统研发必备/OLTP/Speedy_Transactions_in_Multicore_In-Memory_Databases.pdf)
	* [凝视深渊:_千核并发控制评测](./数据库系统研发必备/OLTP/Staring_into_the_Abyss-_An_Evaluation_of_Concurrency_Control_with_One_Thousand_Cores.pdf)
	* [现代面向列的数据库系统的设计与实现](./数据库系统研发必备/OLTP/The_Design_and_Implementation_of_Modern_Column-Oriented_Database_Systems.pdf)
	* [查询执行中的矢量化与编译](./数据库系统研发必备/OLTP/Vectorization_vs._Compilation_in_Query_Execution.pdf)
	* [Volcano:_一个可扩展的并行查询评估系统](./数据库系统研发必备/OLTP/Volcano-An_Extensible_and_Parallel_Query_Evaluation_System.pdf)
	* [为什么您应该运行TPC-DS-A工作负载分析](./数据库系统研发必备/OLTP/Why_You_Should_Run_TPC-DS-A_Workload_Analysis.pdf)


## 来自数据密集型应用设计(DDIA)的论文

## 百篇有意思的机器学习论文
