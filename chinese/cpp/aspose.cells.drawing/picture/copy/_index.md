---
title: Aspose::Cells::Drawing::Picture::Copy method
linktitle: Copy
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::Copy method. Copy the picture in C++.'
type: docs
weight: 600
url: /zh/cpp/aspose.cells.drawing/picture/copy/
---
## Picture::Copy method


Copy the picture.

```cpp
void Aspose::Cells::Drawing::Picture::Copy(const Aspose::Cells::Drawing::Picture &source, const CopyOptions &options)
```


| Parameter | Type | Description |
| --- | --- | --- |
| source | const Aspose::Cells::Drawing::Picture\& | The source picture. |
| options | const CopyOptions\& | The copy options. |


## Examples


```cpp
Aspose::Cells::Startup();
//实例化 Workbook 对象
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//插入第一张图片
int imgIndex1 = worksheet.GetPictures().Add(1, 1, u"1.png");
//获取插入的图片对象
Picture pic1 = worksheet.GetPictures().Get(imgIndex1);
//插入第二张图片
int imgIndex2 = worksheet.GetPictures().Add(1, 9, u"2.jpeg");
//获取插入的图片对象
Picture pic2 = worksheet.GetPictures().Get(imgIndex2);
//将图片 1 复制到图片 2。您将得到两个叠加在一起的图片 1 对象。
CopyOptions opt;
pic2.Copy(pic1, opt);
//保存 Excel 文件。
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Class [CopyOptions](../../../aspose.cells/copyoptions/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
