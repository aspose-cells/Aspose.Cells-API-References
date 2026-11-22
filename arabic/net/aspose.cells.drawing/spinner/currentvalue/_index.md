---
title: "Spinner.CurrentValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Spinner. تحصل أو تعين القيمة الحالية"
type: docs
url: /ar/net/aspose.cells.drawing/spinner/currentvalue/
---
## Spinner.CurrentValue property

يحصل أو يضبط القيمة الحالية.

```csharp
public int CurrentValue { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyCurrentValueDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة عنصر تحكم Spinner
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Spinner, 1, 1, 0, 0, 20, 20);
            Spinner spinner = (Spinner)shape;

            // اضبط خصائص Spinner
            spinner.LinkedCell = "A1";
            spinner.Min = 1;
            spinner.Max = 100;
            spinner.IncrementalChange = 5;
            spinner.CurrentValue = 10; // Using CurrentValue property directly

            // التحقق وإخراج القيمة الحالية
            Console.WriteLine("Spinner CurrentValue: " + spinner.CurrentValue);

            // احفظ المصنف
            workbook.Save("SpinnerDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


