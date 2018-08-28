# LabVIEW-MassData-Smart-Ptr

[lvzmqBus](https://gitee.com/nevstop/lvZmqBus) 中使用的 LabVIEW 大数据模块间传递方案。

![演示](https://images.gitee.com/uploads/images/2018/0822/160314_566fec33_136753.png "屏幕截图.png")

## 支持的数据类型

 - Waveform 
 - Waveform Array
 - Double Array
 - String Array
 
**新增数据类型步骤:**  
 1. 增加新增的数据类型到 "MDPtr TypeDef/MDPtr SupportedDataTypeDef.ctl"
 2. 创建新增数据类型的 DataFrameType。 仿照 "MDPtr TypeDef/MDPtr DataFrame-DoubleArr.ctl"
 3. 仿照 Double Array pack/unpack VI 创建其他数据类型支持
    - 替换内部的 DataFrameType 定义；
    - 注意 pack 需要将数据类型选择为新数据类型；unpack 校验数据类型处需要将待校验数据类型选择为新数据类型。
 4. (可选) 在Polymorphic VI: MDPtr pack.vi/MDPtr Unpack.vi 中，增加新增的 pack/unpack VI。或直接调用新增的 pack/unpack VI。

## 流程说明

参考  **_Example/MDPtr Process Example.vi**   
![输入图片说明](https://images.gitee.com/uploads/images/2018/0828/141100_30fe50a4_136753.png "屏幕截图.png")

## 应用实例

参考  **_Example/MDPtr DAQ Example.vi**
利用 MDPtr 将采集到的 Sine/Square 两个波形数据文件，发送到显示、数据保存两个模块使用。

![FP](https://images.gitee.com/uploads/images/2018/0828/141607_9bd7319a_136753.png "屏幕截图.png")
![BD](https://images.gitee.com/uploads/images/2018/0828/141546_07da7131_136753.png "屏幕截图.png")
