---
title: get_enumerator方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 40
url: /zh/python-net/aspose.cells/unionrange/get_enumerator/
is_root: false
---
##  get_enumerator() {#}
获取此 Range 中单元格的枚举器。


### 返回

细胞计数器


```python
def get_enumerator(self):
    ...
```


### 评论

通过返回的 Enumerator 遍历元素时，cells 集合
不应修改（例如将导致新的 Cell/Row 被实例化或现有的 Cell/Row 被删除的操作）。
否则枚举器可能无法正确遍历所有单元格（某些元素可能会重复遍历或跳过）。


### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [UnionRange](/cells/zh/python-net/aspose.cells/unionrange)
