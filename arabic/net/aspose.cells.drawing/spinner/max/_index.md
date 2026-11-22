---
title: "Spinner.Max"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Spinner. تحصل أو تعين القيمة القصوى لشريط التمرير أو نطاق spinner"
type: docs
url: /ar/net/aspose.cells.drawing/spinner/max/
---
## Spinner.Max property

يحصل أو يضبط القيمة القصوى لنطاق شريط التمرير أو المؤشر.

```csharp
public int Max { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyMaxDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            Aspose.Cells.Drawing.Spinner spinner = sheet.Shapes.AddSpinner(1, 1, 0, 0, 100, 100);
            spinner.Min = 0;
            spinner.Max = 100;
            spinner.IncrementalChange = 5;

            Console.WriteLine($"Spinner Max Value: {spinner.Max}");
        }
    }
}
```

### انظر أيضًا

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


