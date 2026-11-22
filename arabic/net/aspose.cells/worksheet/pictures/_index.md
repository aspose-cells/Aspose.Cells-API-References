---
title: "Worksheet.Pictures"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تحصل على مجموعة Picture"
type: docs
url: /ar/net/aspose.cells/worksheet/pictures/
---
## Worksheet.Pictures property

تحصل على مجموعة [`Picture`](../../../aspose.cells.drawing/picture/).

```csharp
public PictureCollection Pictures { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyPicturesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف صورة إلى ورقة العمل
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            // تعيين خصائص الصورة
            picture.Placement = PlacementType.FreeFloating;
            picture.BorderLineColor = System.Drawing.Color.Blue;
            picture.BorderWeight = 1;

            // احفظ المصنف
            workbook.Save("output.xlsx", SaveFormat.Xlsx);

            // قم بتحميل المصنف المحفوظ للتحقق
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("Number of pictures: " + loadedWorkbook.Worksheets[0].Pictures.Count);
        }
    }
}
```

### انظر أيضًا

* class [PictureCollection](../../../aspose.cells.drawing/picturecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


