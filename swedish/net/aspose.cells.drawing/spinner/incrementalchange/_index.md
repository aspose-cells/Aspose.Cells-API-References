---
title: "Spinner.IncrementalChange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Spinner-egenskap. Hämtar eller anger mängden som rullningslisten eller spinnern ökas per radrullning"
type: docs
url: /sv/net/aspose.cells.drawing/spinner/incrementalchange/
---
## Spinner.IncrementalChange property

Hämtar eller anger mängden som rullningslisten eller spinnern ökas med en radrullning.

```csharp
public int IncrementalChange { get; set; }
```

### Exempel

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

            // Skapa en spinnerkontroll
            Spinner spinner = worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 100);

            // Ange spinner-egenskaper
            spinner.Min = 0;
            spinner.Max = 100;
            spinner.CurrentValue = 50;
            spinner.IncrementalChange = 5; // Demonstrate IncrementalChange property

            // Verifiera och skriv ut värdet för IncrementalChange
            Console.WriteLine("Spinner IncrementalChange: " + spinner.IncrementalChange);

            // Ändra och verifiera igen
            spinner.IncrementalChange = 10;
            Console.WriteLine("Modified IncrementalChange: " + spinner.IncrementalChange);

            // Spara arbetsboken
            workbook.Save("SpinnerIncrementalChangeDemo.xlsx");
        }
    }
}
```

### Se även

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


