---
title: get_style_in_pool方法
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 190
url: /zh/python-net/aspose.cells/workbook/get_style_in_pool/
is_root: false
---
##  get_style_in_pool(index) {#int}
获取样式池中的样式。
工作簿中的所有样式都将汇集到一个池中。
单元格中只有一个简单的参考索引。


### 返回

池中的样式对应于给定的索引，可能为空。


```python
def get_style_in_pool(self, index):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| index | int |索引。|
### 评论

如果返回的样式发生变化，则所有单元格（引用该样式）的样式都会发生变化。


### 也可以看看

* 模块 [aspose.cells](../../)
* 类 [Workbook](/cells/zh/python-net/aspose.cells/workbook)
