---
title: characters方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 50
url: /zh/python-net/aspose.cells.drawing/webextensionshape/characters/
is_root: false
---
##  characters(start_index, length) {#int-int}
返回表示文本中 characters 范围的 Characters 对象。


### 返回

字符对象。


```python
def characters(self, start_index, length):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| start_index | int |字符开始的索引。|
| length | int |字符数。|
### 评论

此方法仅适用于带标题的形状。
### 例子


```python

fontSetting = shape.characters(0, 4)

```



### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [WebExtensionShape](/cells/zh/python-net/aspose.cells.drawing/webextensionshape)
