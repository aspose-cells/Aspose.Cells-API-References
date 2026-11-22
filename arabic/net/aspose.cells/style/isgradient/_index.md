---
title: "Style.IsGradient"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Style. تشير إلى ما إذا كان تظليل الخلية نمطًا تدرجيًا"
type: docs
url: /ar/net/aspose.cells/style/isgradient/
---
## Style.IsGradient property

يشير إلى ما إذا كان تظليل الخلية نمطًا متدرجًا.

```csharp
public bool IsGradient { get; set; }
```

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyIsGradientDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نمط
            Style style = workbook.CreateStyle();
            
            // تعيين خلفية متدرجة
            style.SetTwoColorGradient(Color.LightBlue, Color.DarkBlue, GradientStyleType.Horizontal, 1);
            
            // تطبيق النمط على خلية
            worksheet.Cells["A1"].SetStyle(style);
            
            // تحقق مما إذا كان النمط يحتوي على تدرج
            bool isGradient = worksheet.Cells["A1"].GetStyle().IsGradient;
            
            // أخرج النتيجة.
            Console.WriteLine("Cell A1 style has gradient: " + isGradient);
            
            // احفظ المصنف
            workbook.Save("GradientStyleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


