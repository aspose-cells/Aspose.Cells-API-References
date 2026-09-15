---
title: Aspose::Cells::Drawing::Picture::GetBorderLineColor method
linktitle: GetBorderLineColor
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetBorderLineColor method. Represents the Color of the border line of a picture in C++.'
type: docs
weight: 1100
url: /zh/cpp/aspose.cells.drawing/picture/getborderlinecolor/
---
## Picture::GetBorderLineColor method


Represents the [Color](../../../aspose.cells/color/) of the border line of a picture.

```cpp
Aspose::Cells::Color Aspose::Cells::Drawing::Picture::GetBorderLineColor()
```


## Examples


```cpp
Aspose::Cells::Startup();
//实例化 Workbook 对象
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//在工作表中行列索引为 1 的单元格位置添加图片。该单元格为 "B2"。
int imgIndex = worksheet.GetPictures().Add(1, 1, u"example.jpeg");
//获取插入的图片对象
Picture pic = worksheet.GetPictures().Get(imgIndex);
//设置图片的边框颜色
if (pic.GetBorderLineColor() == Color{ 0xff, 0, 0, 0xff })//Blue
{
    pic.SetBorderLineColor(Color{ 0xff, 0xff, 0, 0 });//Red
}
//保存 Excel 文件。
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
