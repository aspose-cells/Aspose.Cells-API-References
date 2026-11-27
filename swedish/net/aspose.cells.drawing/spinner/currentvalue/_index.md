---
title: "Spinner.CurrentValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Spinner-egenskap. Hämtar eller anger det aktuella värdet"
type: docs
url: /sv/net/aspose.cells.drawing/spinner/currentvalue/
---
## Spinner.CurrentValue property

Hämtar eller anger det aktuella värdet.

```csharp
public int CurrentValue { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en spinner-kontroll
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Spinner, 1, 1, 0, 0, 20, 20);
            Spinner spinner = (Spinner)shape;

            // Ange spinner-egenskaper
            spinner.LinkedCell = "A1";
            spinner.Min = 1;
            spinner.Max = 100;
            spinner.IncrementalChange = 5;
            spinner.CurrentValue = 10; // Using CurrentValue property directly

            // Verifiera och skriv ut det aktuella värdet
            Console.WriteLine("Spinner CurrentValue: " + spinner.CurrentValue);

            // Spara arbetsboken
            workbook.Save("SpinnerDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


