---
title: provider_id 属性
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 80
url: /zh/python-net/aspose.cells.drawing/signatureline/provider_id/
is_root: false
---
## provider_id 属性

获取和设置签名提供者的id。

### 评论

它通常是提供商 com 加载项的 CLSID。

### 例子

```python
from aspose.cells.drawing import SignatureLine
from uuid import uuid4

#  Create signature line object
s2 = SignatureLine()
s2.provider_id = uuid4()

```
### 定义：
```python
@property
def provider_id(self):
    ...
@provider_id.setter
def provider_id(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [SignatureLine](/cells/zh/python-net/aspose.cells.drawing/signatureline)
