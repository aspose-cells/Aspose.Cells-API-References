---
title: "FillFormat.ImageData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FillFormat. تحصل وتعيّن بيانات صورة ImageData"
type: docs
url: /ar/net/aspose.cells.drawing/fillformat/imagedata/
---
## FillFormat.ImageData property

يحصل على بيانات صورة الرسم ويضبطها.

```csharp
public byte[] ImageData { get; set; }
```

### ملاحظات

إذا لم يكن تنسيق التعبئة تنسيق نسيج مخصص، تُرجع null.

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyImageDataDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف صورة عينة إلى ورقة العمل
            string imagePath = "example.png";
            worksheet.Pictures.Add(0, 0, imagePath);

            // أنشئ تعليقًا وحدد بيانات الصورة
            var comment = worksheet.Comments[worksheet.Comments.Add(2, 5)];
            byte[] imageData = File.ReadAllBytes(imagePath);
            comment.CommentShape.Fill.ImageData = imageData;

            // احفظ دفتر العمل
            workbook.Save("FillFormatPropertyImageDataDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


