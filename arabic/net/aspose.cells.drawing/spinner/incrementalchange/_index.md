---
title: "Spinner.IncrementalChange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Spinner. تحصل أو تعين مقدار الزيادة التي يتم فيها تحريك شريط التمرير أو الـ Spinner سطرًا واحدًا"
type: docs
url: /ar/net/aspose.cells.drawing/spinner/incrementalchange/
---
## Spinner.IncrementalChange property

يحصل أو يضبط مقدار الزيادة التي يضيفها شريط التمرير أو المؤشر عند تمرير سطر.

```csharp
public int IncrementalChange { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyIncrementalChangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء عنصر تحكم spinner
            Spinner spinner = worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 100);

            // اضبط خصائص Spinner
            spinner.Min = 0;
            spinner.Max = 100;
            spinner.CurrentValue = 50;
            spinner.IncrementalChange = 5; // Demonstrate IncrementalChange property

            // تحقق وأخرج قيمة IncrementalChange
            Console.WriteLine("Spinner IncrementalChange: " + spinner.IncrementalChange);

            // عدّل وتحقق مرة أخرى
            spinner.IncrementalChange = 10;
            Console.WriteLine("Modified IncrementalChange: " + spinner.IncrementalChange);

            // احفظ المصنف
            workbook.Save("SpinnerIncrementalChangeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


