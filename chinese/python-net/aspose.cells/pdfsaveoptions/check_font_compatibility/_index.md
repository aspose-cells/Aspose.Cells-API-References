---
title: check_font_compatibility 属性
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 80
url: /zh/python-net/aspose.cells/pdfsaveoptions/check_font_compatibility/
is_root: false
---
## check_font_compatibility 属性

指示是否检查文本中每个字符的字体兼容性。

### 评论

默认值是true。
禁用此属性可能会提供更好的性能。
但是当无法使用默认或指定的文本/字符字体来渲染时，
生成的 pdf 中可能会出现不可读的字符（例如块）。
对于这种情况，用户应将此属性保持为 true，以便
可以搜索替代字体并将其用于呈现文本；
### 定义：
```python
@property
def check_font_compatibility(self):
    ...
@check_font_compatibility.setter
def check_font_compatibility(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [PdfSaveOptions](/cells/zh/python-net/aspose.cells/pdfsaveoptions)
