---
title: get_list_value方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 70
url: /zh/python-net/aspose.cells/validation/get_list_value/
is_root: false
---
##  get_list_value(row, column) {#int-int}
获取指定单元格的验证列表的值。


### 返回

为指定单元格生成此验证列表的值。
如果列表引用了一个范围，则返回值将是一个 [ReferredArea](/cells/zh/python-net/aspose.cells/referredarea) 对象；
否则，返回值可能为 null、object[] 或简单对象。


```python
def get_list_value(self, row, column):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| row | int |行索引。|
| column | int |列索引。|
### 评论

仅适用于类型为列表且已应用于给定单元格的验证，
否则将返回 null。


### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [ReferredArea](/cells/zh/python-net/aspose.cells/referredarea)
* 类 [Validation](/cells/zh/python-net/aspose.cells/validation)
