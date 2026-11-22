---
title: "Style.IsTextWrapped"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Style. تحصل أو تعين قيمة تشير إلى ما إذا كان النص داخل الخلية ملفوفًا"
type: docs
url: /ar/net/aspose.cells/style/istextwrapped/
---
## Style.IsTextWrapped property

يحصل على قيمة أو يضبطها تشير إلى ما إذا كان النص داخل الخلية مُلتفًا.

```csharp
public bool IsTextWrapped { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsTextWrappedDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            Cells cells = ws.Cells;
            
            // تعيين نص طويل في الخلية
            Cell cell = cells["A1"];
            cell.PutValue("This is a long text that should be wrapped in the cell");
            
            // تمكين لف النص
            Style style = cell.GetStyle();
            style.IsTextWrapped = true;
            cell.SetStyle(style);
            
            // ضبط ارتفاع الصف لإظهار النص الملفوف
            ws.AutoFitRow(0);
            
            // احفظ المصنف
            wb.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


