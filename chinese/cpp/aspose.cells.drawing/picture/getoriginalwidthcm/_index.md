---
title: Aspose::Cells::Drawing::Picture::GetOriginalWidthCM method
linktitle: GetOriginalWidthCM
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetOriginalWidthCM method. Gets the original width of picture, in unit of centimeters in C++.'
type: docs
weight: 3100
url: /zh/cpp/aspose.cells.drawing/picture/getoriginalwidthcm/
---
## Picture::GetOriginalWidthCM method


Gets the original width of picture, in unit of centimeters.

```cpp
double Aspose::Cells::Drawing::Picture::GetOriginalWidthCM()
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
//获取图片的原始宽度。
double picWidthCM = pic.GetOriginalWidthCM();
//保存 Excel 文件。
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
