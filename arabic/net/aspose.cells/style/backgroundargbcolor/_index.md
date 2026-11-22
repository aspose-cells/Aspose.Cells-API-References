---
title: "Style.BackgroundArgbColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Style. تحصل وتضبط لون الخلفية باستخدام قيمة ARGB 32 بت"
type: docs
url: /ar/net/aspose.cells/style/backgroundargbcolor/
---
## Style.BackgroundArgbColor property

يحصل على اللون الخلفي ويضبطه باستخدام قيمة ARGB 32 بت.

```csharp
public int BackgroundArgbColor { get; set; }
```

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyBackgroundArgbColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Style style = cell.GetStyle();
            style.BackgroundArgbColor = Color.Yellow.ToArgb();
            style.Pattern = BackgroundType.Solid;
            
            cell.SetStyle(style);
            cell.PutValue("Sample Text with Yellow Background");
            
            workbook.Save("BackgroundArgbColorDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


