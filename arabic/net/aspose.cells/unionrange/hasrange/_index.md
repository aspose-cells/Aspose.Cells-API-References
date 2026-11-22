---
title: "UnionRange.HasRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية UnionRange. تشير إلى ما إذا كان هذا يحتوي على نطاق"
type: docs
url: /ar/net/aspose.cells/unionrange/hasrange/
---
## UnionRange.HasRange property

يشير إلى ما إذا كان لهذا نطاق.

```csharp
public bool HasRange { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class UnionRangePropertyHasRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء نطاق اتحاد باستخدام API الصحيح
            UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:A5,B1:B5", 0);
            
            // تحقق مما إذا كان نطاق الاتحاد يحتوي على نطاقات صالحة
            Console.WriteLine("UnionRange has ranges: " + unionRange.HasRange);
            
            // عيّن القيمة والنمط فقط إذا كان النطاق صالحًا
            if (unionRange.HasRange)
            {
                unionRange.Value = "Test Value";
                
                Style style = workbook.CreateStyle();
                style.Pattern = BackgroundType.Solid;
                style.ForegroundColor = System.Drawing.Color.LightBlue;
                unionRange.ApplyStyle(style, new StyleFlag { All = true });
            }
            
            workbook.Save("UnionRangeHasRangeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


