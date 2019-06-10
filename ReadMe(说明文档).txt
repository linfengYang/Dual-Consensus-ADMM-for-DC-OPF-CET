文件夹说明：
SCUC_dat:计算数据。
Picture：一些数据结果图表。


函数文件说明：
DCOPF_ADMM：主函数
ReadDataSCUC：读取SCUC6和SCUC1062数据。
ReadDataDCDOPF:读取DDOPF118.txt和RTS48.txt数据.
SCUC_nodeY:形成导纳矩阵。
partitionNode：分区设定。
partitionDataPI：识别耦合节点和耦合支路。
formMatrixA：等式约束。
formMatrixM：不等式约束。
formQC4Emission：对排放约束按照片区划分。
yanZheng：不分区调用Cplex求解，作为参照值。
formQCP_PI_x_i：构造分块矩阵。


For more detail:http://www.optimization-online.org/DB_HTML/2018/05/6638.html

