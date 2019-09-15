Dual Consensus ADMM for DC-DOPF-CET
================

What about this project/study?（项目介绍）

      This study is using alternating direction method of multipliers (ADMM) approach for solving 
    the direct current dynamic optimal power flow with carbon emission trading (DC-DOPF-CET) problem.
    In this study, we focus on the impact of parameter rou and miu, the number of elements in the 
    consensus variable, the number of subsystems and the scale of power systems on the convergence 
    performance. In order to verify the performance of our proposed algorithms and the effective of improved,
    we apply them on a various of numerical case studies, and compare their key features and simulation results
    with the method in [6] and [7]. The numerical case studies include a 6-bus system, a 30-bus system, a RTS48-bus
    system in [6], a 118-bus system in [7] and a 1062-bus system. The results show that the convergence performance
    largely depends on the number of elements in the consensus variable rather than the number of subsystems or
    the scale of power systems. An excellent subsystem partition strategy cound enhance the convergence performance
    , since it has less global variables.

    [6] A. Kargarian, J. Mohammadi, J. Guo, S. Chakrabarti, M. Barati, G. Hug, S. Kar and R. Baldick, 
        “Toward Distributed/Decentralized DC Optimal Power Flow Implementationin Future Electric Power Systems,”
        IEEE Trans. Smart Grid, 2016.
    [7] Y. Wang, L. Wu and S. Wang, “A Fully-Decentralized Consensus-Based ADMM Approach for DC-OPF With Demand Response,”
        IEEE Trans. Smart Grid, vol. 8, no. 6, pp. 2637-2647, Nov. 2017.


User Guide（用户指南）
-----------

The description of folder (文件夹说明)

    SCUC_dat : The numerical case studies data. 计算数据 

    Picture : The figures and tables in this paper. 数据结果图表。




The description of implement code files  (函数文件说明)

    DCOPF_ADMM.m : The main funciton.  主函数。

    ReadDataSCUC :  Read the SCUC6.txt and SCUC1062.txt.  SCUC6.txt和SCUC1062.txt的读取函数。

    ReadDataDCDOPF : Read the DDOPF118.txt和RTS48.txt.  DDOPF118.txt和RTS48.txt的读取函数。

    SCUC_nodeY :  Construct network admittance matrix. 形成导纳矩阵的函数。

    partitionNode :  Set the partition of the system. 设置分区的函数。

    partitionDataPI :  The procedure of identifying "real" coupling boudnary branches and brandary buses. 识别耦合节点和耦合支路的函数。

    formMatrixA :  Corresponding to the constraint (17) in manuscript. 构造文章中约束(17)的系数矩阵。

    formMatrixM :  Corresponding to the constraint (18) in manuscript. 构造文章中约束(18)的系数矩阵。

    formQC4Emission : Corresponding to the constraint (19) in manuscript.  构造文章中约束(19)的系数矩阵。

    yanZheng :  Using Cplex to solve DC-DOPF-CET problem. 使用Cplex求解DC-DOPF-CET。

    formQCP_PI_x_i : Corresponding to the constraint (30) in manuscript. 构造文章中约束(30)的系数矩阵。





Prerequisite(运行该项目需要的库或软件等):
-----------

    Matlab R2014a
    Cplex 12.6.2




Publication:
-----------
    If you use our study in academic work then please consider citing our papers.
    (如果您参考我们的项目/论文 并用于学术目的，请考虑引用我们的论文




About Us (关于我们)
-----------
    Authors：Lingfeng Yang (ylf@gxu.edu.cn),Jiangyao Luo (landiljy@163.com),Yan Xu,Zhenrong Zhang,Zhaoyang Dong
    Team：www.scholat.com/team/eidp
    Webpage: http://jians.gxu.edu.cn/default.do
