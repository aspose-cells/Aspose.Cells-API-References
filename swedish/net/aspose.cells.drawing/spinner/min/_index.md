---
title: "Spinner.Min"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Spinner-egenskap. Hämtar eller anger det minsta värdet för en rullningslist eller spinner-intervall"
type: docs
url: /sv/net/aspose.cells.drawing/spinner/min/
---
## Spinner.Min property

Hämtar eller anger det minsta värdet för ett rullningslist‑ eller spinnerintervall.

```csharp
public int Min { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en spinner-kontroll med korrekta dimensioner
            Spinner spinner = worksheet.Shapes.AddSpinner(1, 1, 1, 1, 100, 20);

            // Ställ in spinner-egenskaper inklusive Min
            spinner.Min = 10;
            spinner.Max = 100;
            spinner.IncrementalChange = 5;
            spinner.CurrentValue = 15;

            // Verifiera och skriv ut Min-egenskapen
            Console.WriteLine("Spinner Min Value: " + spinner.Min);

            // Spara arbetsboken
            workbook.Save("SpinnerPropertyMinDemo.xlsx");
        }
    }
}
```

### Se även

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


