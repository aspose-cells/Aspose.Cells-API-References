---
title: "Worksheet.BackgroundImage"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تحصل على صورة خلفية ورقة العمل وتضبطها"
type: docs
url: /ar/net/aspose.cells/worksheet/backgroundimage/
---
## Worksheet.BackgroundImage property

يحصل أو يعيّن صورة خلفية ورقة العمل.

```csharp
public byte[] BackgroundImage { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyBackgroundImageDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // احصل على ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // مسار ملف الصورة
            string imagePath = "background.jpg";
            
            // قراءة ملف الصورة إلى مصفوفة بايت
            byte[] imageData = File.ReadAllBytes(imagePath);
            
            // تعيين صورة الخلفية لورقة العمل
            worksheet.BackgroundImage = imageData;
            
            // احفظ المصنف
            workbook.Save("WorksheetWithBackground.xlsx");
            
            Console.WriteLine("Worksheet background image set successfully.");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


