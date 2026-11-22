---
title: "PageSetup.LeftMargin"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تمثل حجم الهامش الأيسر بوحدة السنتيمترات"
type: docs
url: /ar/net/aspose.cells/pagesetup/leftmargin/
---
## PageSetup.LeftMargin property

يمثل حجم الهامش الأيسر، بوحدة السنتيمترات.

```csharp
public double LeftMargin { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyLeftMarginDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // قم بتعيين بعض البيانات النموذجية
            sheet.Cells["A1"].PutValue("Left Margin Demonstration");
            sheet.Cells["A2"].PutValue("This shows how to set page margins");

            // ضبط الهامش الأيسر (بالبوصة)
            sheet.PageSetup.LeftMargin = 1.5;

            // اطبع قيمة الهامش الأيسر إلى وحدة التحكم
            Console.WriteLine("Left Margin set to: " + sheet.PageSetup.LeftMargin + " inches");

            // احفظ إلى PDF لتوضيح الهامش
            string outputPath = "LeftMarginDemo.pdf";
            workbook.Save(outputPath, SaveFormat.Pdf);

            Console.WriteLine("File saved with left margin: " + outputPath);
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


