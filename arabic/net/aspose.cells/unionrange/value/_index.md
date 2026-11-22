---
title: "UnionRange.Value"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية UnionRange. تحصل وتعيّن قيم النطاق"
type: docs
url: /ar/net/aspose.cells/unionrange/value/
---
## UnionRange.Value property

يحصل على قيم النطاق ويضبطها.

```csharp
public object Value { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class UnionRangePropertyValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء نطاق اتحاد باستخدام API الصحيح
            UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:B2,D1:E2", 0);
            
            // تعيين قيمة للنطاق الاتحاد بالكامل
            unionRange.Value = "Test Value";
            
            // إنشاء وتطبيق النمط
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            unionRange.ApplyStyle(style, new StyleFlag { All = true });
            
            // احفظ المصنف
            workbook.Save("UnionRangeValueDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


