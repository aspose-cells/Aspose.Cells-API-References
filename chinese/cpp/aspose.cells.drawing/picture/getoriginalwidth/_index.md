---
title: Aspose::Cells::Drawing::Picture::GetOriginalWidth method
linktitle: GetOriginalWidth
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetOriginalWidth method. Gets the original width of the picture in C++.'
type: docs
weight: 1000
url: /zh/cpp/aspose.cells.drawing/picture/getoriginalwidth/
---
## Picture::GetOriginalWidth method


Gets the original width of the picture.

```cpp
int32_t Aspose::Cells::Drawing::Picture::GetOriginalWidth()
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
int picWidth = pic.GetOriginalWidth();
//保存 Excel 文件。
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
