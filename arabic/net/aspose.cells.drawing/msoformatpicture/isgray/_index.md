---
title: "MsoFormatPicture.IsGray"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MsoFormatPicture. تشير إلى ما إذا كانت هذه الصورة يجب أن تُعرض بالأبيض والأسود"
type: docs
url: /ar/net/aspose.cells.drawing/msoformatpicture/isgray/
---
## MsoFormatPicture.IsGray property

يشير إلى ما إذا كان يجب عرض هذه الصورة بتدرج الرمادي.

```csharp
public bool IsGray { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyIsGrayDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكل صورة
            using (Stream imageStream = File.OpenRead("example.gif"))
            {
                Shape shape = worksheet.Shapes.AddPicture(0, 0, imageStream, 100, 100);
                
                // اضبط خصائص تنسيق الصورة
                shape.FormatPicture.Brightness = 90;
                shape.FormatPicture.Contrast = 90;
                shape.FormatPicture.IsGray = true;

                // احفظ المصنف
                workbook.Save("output.xlsx");
            }

            // أعد التحميل وتحقق من الخصائص
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            
            Console.WriteLine("Brightness: " + loadedShape.FormatPicture.Brightness);
            Console.WriteLine("Contrast: " + loadedShape.FormatPicture.Contrast);
            Console.WriteLine("IsGray: " + loadedShape.FormatPicture.IsGray);
        }
    }
}
```

### انظر أيضًا

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


