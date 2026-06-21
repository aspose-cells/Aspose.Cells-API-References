---
title: Aspose::Cells::Drawing::Picture::GetBorderWeight method
linktitle: GetBorderWeight
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetBorderWeight method. Gets or sets the weight of the border line of a picture in units of pt in C++.'
type: docs
weight: 1300
url: /ar/cpp/aspose.cells.drawing/picture/getborderweight/
---
## Picture::GetBorderWeight method


Gets or sets the weight of the border line of a picture in units of pt.

```cpp
double Aspose::Cells::Drawing::Picture::GetBorderWeight()
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
pic.SetBorderLineColor(Color{ 0xff, 0xff, 0, 0 });//Red
//تعيين عرض حد الصورة
if (pic.GetBorderWeight() == 3)
{
    pic.SetBorderWeight(3);
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
