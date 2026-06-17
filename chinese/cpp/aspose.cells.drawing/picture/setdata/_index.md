---
title: Aspose::Cells::Drawing::Picture::SetData method
linktitle: SetData
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::SetData method. Gets the data of the picture in C++.'
type: docs
weight: 1600
url: /zh/cpp/aspose.cells.drawing/picture/setdata/
---
## Picture::SetData method


Gets the data of the picture.

```cpp
void Aspose::Cells::Drawing::Picture::SetData(const Vector<uint8_t> &value)
```


## Examples


```cpp
Aspose::Cells::Startup();
//实例化 Workbook 对象
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//插入第一张图片
int imgIndex1 = worksheet.GetPictures().Add(1, 1, u"example1.png");
//获取插入的图片对象
Picture pic1 = worksheet.GetPictures().Get(imgIndex1);
//插入第二张图片
int imgIndex2 = worksheet.GetPictures().Add(1, 9, u"example2.jpeg");
//获取插入的图片对象
Picture pic2 = worksheet.GetPictures().Get(imgIndex2);
//将第一张图像的字节数据分配给第二张图像
pic2.SetData(pic1.GetData());
//保存 Excel 文件。
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
