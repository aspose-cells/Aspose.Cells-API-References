---
title: set_metered_key方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 40
url: /zh/python-net/aspose.cells/metered/set_metered_key/
is_root: false
---
##  set_metered_key(public_key, private_key) {#str-str}
设置计量公钥和私钥。
如果你购买了metered license，在开始申请的时候，应该调用这个API，一般情况下，这个就够了。但是，如果总是上传消费数据失败，超过24小时，license会被设置为评估状态，为避免这种情况，您应该定期检查license状态，如果是评估状态，请再次拨打此API。



```python
def set_metered_key(self, public_key, private_key):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| public_key | str |公钥|
| private_key | str |私钥|



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Metered](/cells/zh/python-net/aspose.cells/metered)
