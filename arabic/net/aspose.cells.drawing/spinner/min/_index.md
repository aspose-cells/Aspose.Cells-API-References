---
title: "Spinner.Min"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Spinner. تحصل أو تعين القيمة الدنيا لشريط التمرير أو نطاق الـ Spinner"
type: docs
url: /ar/net/aspose.cells.drawing/spinner/min/
---
## Spinner.Min property

يحصل أو يضبط القيمة الدنيا لنطاق شريط التمرير أو المؤشر.

```csharp
public int Min { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyMinDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة عنصر تحكم Spinner بأبعاد مناسبة
            Spinner spinner = worksheet.Shapes.AddSpinner(1, 1, 1, 1, 100, 20);

            // تعيين خصائص الـ Spinner بما في ذلك Min
            spinner.Min = 10;
            spinner.Max = 100;
            spinner.IncrementalChange = 5;
            spinner.CurrentValue = 15;

            // التحقق وإخراج خاصية Min
            Console.WriteLine("Spinner Min Value: " + spinner.Min);

            // احفظ المصنف
            workbook.Save("SpinnerPropertyMinDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


