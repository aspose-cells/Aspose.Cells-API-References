---
title: "StyleFlag.All"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية StyleFlag. سيتم تطبيق جميع الخصائص"
type: docs
url: /ar/net/aspose.cells/styleflag/all/
---
## StyleFlag.All property

سيتم تطبيق جميع الخصائص.

```csharp
public bool All { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyAllDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // إنشاء نمط بخلفية حمراء صلبة
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.Red;

            // إنشاء علم نمط مع ضبط خاصية All على true
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.All = true;

            // تطبيق النمط على العمود الأول
            Column column = cells.Columns[0];
            column.ApplyStyle(style, styleFlag);

            // التحقق من تطبيق النمط على الخلايا في العمود
            Cell cell = cells[0, 0];
            Style appliedStyle = cell.GetStyle();
            
            Console.WriteLine("Pattern: " + appliedStyle.Pattern);
            Console.WriteLine("Color: " + appliedStyle.ForegroundColor);
        }
    }
}
```

### انظر أيضًا

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


