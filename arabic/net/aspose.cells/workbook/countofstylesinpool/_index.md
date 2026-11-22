---
title: "Workbook.CountOfStylesInPool"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Workbook. تحصل على عدد الأنماط في مجموعة الأنماط"
type: docs
url: /ar/net/aspose.cells/workbook/countofstylesinpool/
---
## Workbook.CountOfStylesInPool property

يحصل على عدد الأنماط في مجموعة الأنماط.

```csharp
public int CountOfStylesInPool { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyCountOfStylesInPoolDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            
            // احصل على العدد الأولي للأنماط في المجموعة
            int initialStyleCount = wb.CountOfStylesInPool;
            Console.WriteLine($"Initial styles in pool: {initialStyleCount}");

            // أضف بعض الأنماط عن طريق تعديل الخلايا
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // النمط 1
            Style style1 = wb.CreateStyle();
            style1.Font.Name = "Arial";
            style1.Font.Size = 12;
            cells["A1"].SetStyle(style1);
            
            // النمط 2
            Style style2 = wb.CreateStyle();
            style2.Font.Color = System.Drawing.Color.Red;
            style2.Pattern = BackgroundType.Solid;
            cells["B1"].SetStyle(style2);

            // احصل على العدد المحدث للأنماط
            int updatedStyleCount = wb.CountOfStylesInPool;
            Console.WriteLine($"Styles after modifications: {updatedStyleCount}");

            // احفظ لتوضيح استمرارية الأنماط
            wb.Save("output.html", SaveFormat.Html);
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


