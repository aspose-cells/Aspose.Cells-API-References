---
title: "PictureCollection.Camera"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PictureCollection. تأخذ صورة للنطاق"
type: docs
url: /ar/net/aspose.cells.drawing/picturecollection/camera/
---
## PictureCollection.Camera method

يأخذ صورة للنطاق.

```csharp
public int Camera(int row, int column, string range)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف لهذه الصورة. |
| عمود | Int32 | فهرس العمود لهذه الصورة. |
| نطاق | String | المنطقة التي تتطلب التصوير |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class PictureCollectionMethodCameraWithInt32Int32StringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات النموذجية لإنشاء نطاق
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "More Data";
            worksheet.Cells["A2"].Value = "Row 2";
            worksheet.Cells["B2"].Value = "Row 2 Col 2";

            try
            {
                // احصل على مجموعة Pictures من ورقة العمل
                PictureCollection pictures = worksheet.Pictures;

                // استدعِ طريقة Camera لإنشاء صورة كاميرا
                // المعلمات: row (الصف العلوي الأيسر)، column (العمود العلوي الأيسر)، range (نطاق المصدر)
                int pictureIndex = pictures.Camera(5, 1, "A1:B2");

                Console.WriteLine($"Camera picture added successfully at index: {pictureIndex}");

                // احفظ المصنف
                workbook.Save("CameraDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling Camera method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


