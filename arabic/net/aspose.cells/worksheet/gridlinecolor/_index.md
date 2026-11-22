---
title: "Worksheet.GridlineColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تحصل وتعيّن لون خطوط الشبكة"
type: docs
url: /ar/net/aspose.cells/worksheet/gridlinecolor/
---
## Worksheet.GridlineColor property

يحصل على ويضبط لون خطوط الشبكة.

```csharp
public Color GridlineColor { get; set; }
```

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyGridlineColorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين لون خطوط الشبكة إلى الأحمر
            worksheet.GridlineColor = Color.Red;
            
            // احفظ المصنف
            string outputPath = "GridlineColorDemo.xlsx";
            workbook.Save(outputPath);
            
            Console.WriteLine("Gridline color set to red and saved to: " + outputPath);
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


