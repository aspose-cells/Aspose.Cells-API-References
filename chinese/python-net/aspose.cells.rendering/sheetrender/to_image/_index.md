---
title: to_image方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 40
url: /zh/python-net/aspose.cells.rendering/sheetrender/to_image/
is_root: false
---
##  to_image(page_index, file_name) {#int-str}
将特定页面渲染到文件中。



```python
def to_image(self, page_index, file_name):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| page_index | int |指示要转换的页面|
| file_name | str |输出图像的文件名|

### 例子

以下代码将第一张纸的第一页输出为 png 图像。

```python
from aspose.cells import Workbook
from aspose.cells.drawing import ImageType
from aspose.cells.rendering import ImageOrPrintOptions, SheetRender

# load the source file with images.
wb = Workbook("Book1.xlsx")
imgOpt = ImageOrPrintOptions()
# set output image type.
imgOpt.image_type = ImageType.PNG
# render the first sheet.
sr = SheetRender(wb.worksheets[0], imgOpt)
# output the first page of the sheet to image.
sr.to_image(0, "output.png")

```


##  to_image(page_index, stream) {#int-io.RawIOBase}
将特定页面渲染到流中。



```python
def to_image(self, page_index, stream):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| page_index | int |指示要转换的页面|
| stream | io.RawIOBase |输出图像流|



### 也可以看看
* 模块 [aspose.cells.rendering](../../)
* 类 [SheetRender](/cells/zh/python-net/aspose.cells.rendering/sheetrender)
