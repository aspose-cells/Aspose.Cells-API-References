---
title: tiff_color_depth 属性
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 340
url: /zh/python-net/aspose.cells.rendering/imageorprintoptions/tiff_color_depth/
is_root: false
---
## tiff_color_depth 属性

获取或设置位深度以仅在将页面保存为 `Tiff` 格式时应用。

### 评论

仅在保存到 TIFF 时有效。
如果TiffCompression设置为CCITT3、CCITT4，这个不会生效，生成的tiff图片的位深会一直为1。
### 定义：
```python
@property
def tiff_color_depth(self):
    ...
@tiff_color_depth.setter
def tiff_color_depth(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells.rendering](../../)
* 类 [ColorDepth](/cells/zh/python-net/aspose.cells.rendering/colordepth)
* 类 [ImageOrPrintOptions](/cells/zh/python-net/aspose.cells.rendering/imageorprintoptions)
