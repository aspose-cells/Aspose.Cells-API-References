---
title: Metered类
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 1050
url: /zh/python-net/aspose.cells/metered/
is_root: false
---
## Metered类
提供设置计量键的方法。



Metered 类型公开了以下成员：

### 构造器
|构造器|描述|
| :- | :- |
| [Metered()](/cells/zh/python-net/aspose.cells/metered/__init__/#) |初始化此类的新实例。|


### 方法
|方法|描述|
| :- | :- |
| [set_metered_key(public_key, private_key)](/cells/zh/python-net/aspose.cells/metered/set_metered_key/#str-str) |设置计量公钥和私钥。<br/>如果你购买了metered license，在开始申请的时候，应该拨打这个API，一般来说，这个就可以了。你应该定期查看license状态，如果是评估状态，再拨打这个API。|
| [get_consumption_quantity()](/cells/zh/python-net/aspose.cells/metered/get_consumption_quantity/#) |获取消费文件大小|
| [get_consumption_credit()](/cells/zh/python-net/aspose.cells/metered/get_consumption_credit/#) |获得消费信用|



### 例子

在此示例中，将尝试设置计量公钥和私钥


```python
from aspose.cells import Metered

matered = Metered()
matered.set_metered_key("PublicKey", "PrivateKey")

```

### 也可以看看
* 模块 [aspose.cells](..)
