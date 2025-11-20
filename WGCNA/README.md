
WGCNA Input
1. 文件列表

本项目的 WGCNA 分析需要 两个输入文件：
	1.	starting_expression.txt
基因表达矩阵（行＝基因，列＝样本）
	2.	starting_info.txt
样本注释文件（行＝样本，列＝表型信息）
2. starting_expression.txt（表达矩阵）

文件格式要求
	•	行名（第一列）必须为基因 ID
	•	列名（第一行）必须为样本 ID
	•	所有表达值需为数值型
	•	不允许空值（NA）
	•	行列顺序可以任意，但必须和样本信息文件一一对应

  GeneID       GSM1620759   GSM1620760   GSM1620761   ...
ZZZ3         9.23         9.42         8.98         ...
ZYX          10.76        10.41        10.21        ...
...

3. starting_info.txt（样本注释）

文件格式要求
	•	行名（第一列）为样本 ID，与表达矩阵列名完全一致
	•	至少包含 1 列分类变量（用于 WGCNA trait 相关性分析）
	•	列数可以≥1
	•	文本文件建议以 TAB 分隔

  sample        Group
GSM1620759    control
GSM1620760    control
GSM1620761    control
...



Its a copy for https://github.com/RajNINDS/V321L_DG/blob/main/Rcode_wgcna.txt  from Neuregulin1 Nuclear Signaling Influences Adult Neurogenesis and Regulates a Schizophrenia Susceptibility Gene Network within the Mouse Dentate Gyrus  and use nathanprovin/docker_wgcna:1.4 docker to run
