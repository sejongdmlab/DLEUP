# DLEUP

This article provides executables of all frameworks and all datasets used in our research of Damped Erasable Utility Pattern Mining.

The executables include all the frameworks, such as DLEUP, DWEL\*+, EPAS\*+, LEUM, DEPL+, and MED+, and all the datasets which are used in our experiment: Connect, Pumsb, Retail, Foodmart, OnlineRetail, E-Shop, and T10I4DxK.

All executables were compiled to run on 64-bit architectures.

Please refer to the following guide:

1. Note that the name of the executable for each algorithm is as follows:

| Original Name   | DLEUP | DWEL\*+ | EPAS\*+  | LEUM | DEPL+ | MED+ |
| --------------- | ----- | ------- | -------- | ---- | ----- | ---- |
| Executable Name | DLEUP | DWEL+   | EPAS+    | LEUM | DEPL+ | MED+ |

Note that the symbol "*" cannot be used in file names. The executable is named without it.

2. The parameters of the executables are as follows:

For DLEUP, DWEL\*+, DEPL+, and MED+
```bash
[0]          [1]            [2]                       [3]                                [4]
[Executable] [Threshold(%)] [Utility Data Path(.txt)] [Transaction Data File Path(.txt)] [Decaying-Factor]
```

For EPAS\*+ and LEUM
```bash
[0]          [1]            [2]                       [3]                                [4]
[Executable] [Threshold(%)] [Utility Data Path(.txt)] [Transaction Data File Path(.txt)] [DivNum]
```

3. Next, the file name and the parameters of each dataset are as follows:

|  Dataset      | Database Size      | Number of Items | Average Transaction Length |
| ------------- | -------------------| --------------- | -------------------------- |
| Connect       | 67,557             | 129             | 43.0                       |
| Pumsb         | 49,046             | 2,113           | 74.0                       |
| Retail        | 88,162             | 16,470          | 10.3                       |
| Foodmart      | 36,869             | 1,560           | 4.45                       |
| OnlineRetail  | 530,104            | 7,918           | 6.8                        |
| E-Shop        | 165,474	           | 24,564          | 13                         |
| T10I4DxK      | 200,000–1,000,000  | 1,000           | 10.0                       |


4. For example
```bash
DLEUP 0.019 ..\Data\utilPumsb.txt ..\Data\Pumsb.txt 0.99998

```
will run DLEUP on Pumsb with the maximum gain threshold set to 0.019% and the decaying factor set to 0.99998.
```bash
LEUM 70 ..\Data\utilConnect.txt ..\Data\Connect.txt 10
```
will run LEUM on Connect with the maximum gain threshold set to 70% and the division number set to 10.