---
title: "Style.Pattern"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Style. تحصل أو تعين نوع نمط خلفية الخلية"
type: docs
url: /ar/net/aspose.cells/style/pattern/
---
## Style.Pattern property

يحصل على نوع نمط خلفية الخلية أو يضبطه.

```csharp
public BackgroundType Pattern { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyPatternDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // الوصول إلى الخلية والحصول على نمطها
            Cell cell = cells[0, 0];
            Style style = cell.GetStyle();
            
            // تعيين النمط ولون المقدمة
            style.Pattern = BackgroundType.Gray50;
            style.ForegroundColor = System.Drawing.Color.LightGray;
            
            // تطبيق النمط على الخلية
            cell.SetStyle(style);
            
            // احفظ المصنف
            workbook.Save("PatternPropertyDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [BackgroundType](../../backgroundtype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


