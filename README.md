# LabVIEW-MassData-Smart-Ptr

[![Check_Broken_VIs](https://github.com/NEVSTOP-LAB/LabVIEW-MassData-Smart-Ptr/actions/workflows/Check_Broken_VIs.yml/badge.svg)](https://github.com/NEVSTOP-LAB/LabVIEW-MassData-Smart-Ptr/actions/workflows/Check_Broken_VIs.yml)
[![Build_VIPM_Library](https://github.com/NEVSTOP-LAB/LabVIEW-MassData-Smart-Ptr/actions/workflows/Build_VIPM_Library.yml/badge.svg)](https://github.com/NEVSTOP-LAB/LabVIEW-MassData-Smart-Ptr/actions/workflows/Build_VIPM_Library.yml)

![演示](https://images.gitee.com/uploads/images/2018/0822/160314_566fec33_136753.png "屏幕截图.png")

## 支持的数据类型

 - Memory (任意数据 Flattern To String 后，进行传输)
 
## 流程说明

参考 `_Example/MDPtr Process Example.vi`     

![image](https://user-images.githubusercontent.com/8196752/120073784-68db5c80-c0cc-11eb-9906-d7de478bd6b1.png)

## 应用实例

参考 `_Example/MDPtr DAQ Example.vi`    

利用 MDPtr 将采集到的 Sine/Square 两个波形数据文件，发送到显示、数据保存两个模块使用。   

后面板逻辑：    
![image](https://user-images.githubusercontent.com/8196752/120073829-932d1a00-c0cc-11eb-8779-8229187e1c61.png)
