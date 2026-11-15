---
title: Aspose::Cells::Drawing::Picture::SetBorderWeight method
linktitle: SetBorderWeight
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::SetBorderWeight method. Gets or sets the weight of the border line of a picture in units of pt in C++.'
type: docs
weight: 1600
url: /ar/cpp/aspose.cells.drawing/picture/setborderweight/
---
## Picture::SetBorderWeight method


Gets or sets the weight of the border line of a picture in units of pt.

```cpp
void Aspose::Cells::Drawing::Picture::SetBorderWeight(double value)
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
//تعيين لون حد الصورة
pic.SetBorderLineColor(Color{ 0xff, 0xff, 0, 0 });//Red
//تعيين عرض حد الصورة
if (pic.GetBorderWeight() == 3)
{
    pic.SetBorderWeight(3);
}
//احفظ ملف Excel.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
