---
title: Aspose::Cells::Drawing::Picture::GetOriginalWidthCM method
linktitle: GetOriginalWidthCM
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetOriginalWidthCM method. Gets the original width of picture, in unit of centimeters in C++.'
type: docs
weight: 3300
url: /ar/cpp/aspose.cells.drawing/picture/getoriginalwidthcm/
---
## Picture::GetOriginalWidthCM method


Gets the original width of picture, in unit of centimeters.

```cpp
double Aspose::Cells::Drawing::Picture::GetOriginalWidthCM()
```


## Examples


```cpp
Aspose::Cells::Startup();
//إنشاء كائن Workbook
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//إضافة صورة في موقع خلية ذات مؤشرات الصف والعمود 1 في ورقة العمل. هي الخلية "B2"
int imgIndex = worksheet.GetPictures().Add(1, 1, u"example.jpeg");
//احصل على كائن الصورة المدخلة
Picture pic = worksheet.GetPictures().Get(imgIndex);
//يحصل على العرض الأصلي للصورة.
double picWidthCM = pic.GetOriginalWidthCM();
//احفظ ملف Excel.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
