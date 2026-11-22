---
title: "MsoFormatPicture.IsBiLevel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "MsoFormatPicture property. يشير إلى ما إذا كان يجب عرض هذه الصورة بالأبيض والأسود ثنائي اللون"
type: docs
url: /ar/net/aspose.cells.drawing/msoformatpicture/isbilevel/
---
## MsoFormatPicture.IsBiLevel property

يشير إلى ما إذا كان يجب عرض هذه الصورة بالأبيض والأسود ثنائي اللون.

```csharp
public bool IsBiLevel { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyIsBiLevelDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف صورة إلى ورقة العمل
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[index];
            
            // حدد الصورة إلى ثنائي المستوى (أبيض وأسود)
            picture.FormatPicture.IsBiLevel = true;
            
            // تحقق واطبع قيمة الخاصية IsBiLevel
            Console.WriteLine("Picture is bi-level: " + picture.FormatPicture.IsBiLevel);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


