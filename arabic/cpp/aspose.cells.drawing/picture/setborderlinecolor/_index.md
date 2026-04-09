---
title: Aspose::Cells::Drawing::Picture::SetBorderLineColor method
linktitle: SetBorderLineColor
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::SetBorderLineColor method. Represents the Color of the border line of a picture in C++.'
type: docs
weight: 1200
url: /ar/cpp/aspose.cells.drawing/picture/setborderlinecolor/
---
## Picture::SetBorderLineColor method


Represents the [Color](../../../aspose.cells/color/) of the border line of a picture.

```cpp
void Aspose::Cells::Drawing::Picture::SetBorderLineColor(const Aspose::Cells::Color &value)
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
//تعيين لون حد الصورة
if (pic.GetBorderLineColor() == Color{ 0xff, 0, 0, 0xff })//Blue
{
    pic.SetBorderLineColor(Color{ 0xff, 0xff, 0, 0 });//Red
}
//Save the excel file.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
