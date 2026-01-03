# 数据挖掘期末作业
## CSIRO - Image2Biomass Prediction
数据集下载 https://www.kaggle.com/competitions/csiro-biomass/data
- 核心任务：
  - 根据牧场照片（Images）和元数据（Metadata），预测 5 个具体的生物量指标（Target Biomass Components）。

- 预测目标 (Targets)：

        Dry_Green_g: 干绿色植被（不含三叶草） 

        Dry_Dead_g: 干枯死物质

        Dry_Clover_g: 干三叶草生物量

        GDM_g: 绿色干物质 (Green Dry Matter) 

        Dry_Total_g: 总干生物量 

- 输入数据：

    图像: 牧场的草地照片。

    表格数据:

        Pre_GSHH_NDVI: 植被指数 (NDVI)。

        Height_Ave_cm: 平均高度。

        Sampling_Date: 采样日期 (不仅是时间特征，还隐含季节信息)。

        State: 所在的州 (地理位置信息)。 

        Species: 牧草种类。
## 第一阶段：数据清洗与 EDA (探索性数据分析)

```
# 1. 创建名为 csiro 的环境，指定 python 3.10
conda create -n csiro python=3.10 -y

# 2. 激活环境
conda activate csiro

# 3. 安装基础数据科学包 (对应第一阶段)
pip install pandas numpy matplotlib seaborn scikit-learn jupyterlab
```

## 第二阶段：
```
pip install lightgbm 
```
## 第三阶段：
```
conda install pytorch torchvision -c pytorch
pip install tqdm ipywidgets
```