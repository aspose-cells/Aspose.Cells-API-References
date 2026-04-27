---
title: Aspose::Cells::Drawing::Picture::GetOriginalHeightInch method
linktitle: GetOriginalHeightInch
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetOriginalHeightInch method. Gets the original height of picture, in unit of inches in C++.'
type: docs
weight: 3200
url: /ar/cpp/aspose.cells.drawing/picture/getoriginalheightinch/
---
## Picture::GetOriginalHeightInch method


Gets the original height of picture, in unit of inches.

```cpp
double Aspose::Cells::Drawing::Picture::GetOriginalHeightInch()
```


## Examples


```cpp
Aspose::Cells::Startup();
//إنشاء كائن Workbook
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//إضافة صورة في موقع الخلية التي مؤشرات الصف والعمود لها 1 في ورقة العمل. إنها الخلية "B2"
int imgIndex = worksheet.GetPictures().Add(1, 1, u"example.jpeg");
//احصل على كائن الصورة المُدرَج
Picture pic = worksheet.GetPictures().Get(imgIndex);
//يحصل على الارتفاع الأصلي للصورة.
double picHeightInch = pic.GetOriginalHeightInch();
//Save the excel file.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
