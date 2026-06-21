---
title: Aspose::Cells::Drawing::Picture::GetData method
linktitle: GetData
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetData method. Gets the data of the picture in C++.'
type: docs
weight: 1500
url: /ar/cpp/aspose.cells.drawing/picture/getdata/
---
## Picture::GetData method


Gets the data of the picture.

```cpp
Vector<uint8_t> Aspose::Cells::Drawing::Picture::GetData()
```


## Examples


```cpp
Aspose::Cells::Startup();
//إنشاء كائن Workbook
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//إدراج الصورة الأولى
int imgIndex1 = worksheet.GetPictures().Add(1, 1, u"example1.png");
//احصل على كائن الصورة المُدرَج
Picture pic1 = worksheet.GetPictures().Get(imgIndex1);
//إدراج الصورة الثانية
int imgIndex2 = worksheet.GetPictures().Add(1, 9, u"example2.jpeg");
//احصل على كائن الصورة المُدرَج
Picture pic2 = worksheet.GetPictures().Get(imgIndex2);
//تعيين بيانات البايت للصورة الأولى إلى الصورة الثانية
pic2.SetData(pic1.GetData());
//Save the excel file.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
