---
title: to_image方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 210
url: /zh/python-net/aspose.cells.drawing/commentshape/to_image/
is_root: false
---
##  to_image(stream, image_type) {#io.RawIOBase-ImageType}
创建形状图像并将其保存到指定格式的流中。



```python
def to_image(self, stream, image_type):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| stream | io.RawIOBase |输出流。|
| image_type | [ImageType](/cells/zh/python-net/aspose.cells.drawing/imagetype) |保存图像的类型。|
### 评论

支持以下格式：
.bmp、.gif、.jpg、.jpeg、.tiff、.emf。
### 例子

```python
from aspose.cells.drawing import ImageType
from io import BytesIO

imageStream = BytesIO()
shape.to_image(imageStream, ImageType.PNG)

```


##  to_image(image_file, options) {#str-aspose.cells.rendering.ImageOrPrintOptions}
将形状保存到文件中。



```python
def to_image(self, image_file, options):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| image_file | str |  |
| options | aspose.cells.rendering.ImageOrPrintOptions |  |

### 例子

```python
from aspose.cells.rendering import ImageOrPrintOptions

op = ImageOrPrintOptions()
shape.to_image("exmaple.png", op)

```


##  to_image(stream, options) {#io.RawIOBase-aspose.cells.rendering.ImageOrPrintOptions}
将形状保存到流中。



```python
def to_image(self, stream, options):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| stream | io.RawIOBase |  |
| options | aspose.cells.rendering.ImageOrPrintOptions |  |

### 例子

```python
from aspose.cells.rendering import ImageOrPrintOptions
from io import BytesIO

imageStream = BytesIO()
op = ImageOrPrintOptions()
shape.to_image(imageStream, op)

```



### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [CommentShape](/cells/zh/python-net/aspose.cells.drawing/commentshape)
