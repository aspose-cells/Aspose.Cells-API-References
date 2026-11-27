---
title: "Spinner.Shadow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Spinner-egenskap. Anger om formen har 3D-skuggning"
type: docs
url: /sv/net/aspose.cells.drawing/spinner/shadow/
---
## Spinner.Shadow property

Anger om formen har 3‑D‑skuggning.

```csharp
public bool Shadow { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SpinnerPropertyShadowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en spinner i kalkylbladet
            Spinner spinner = worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 30);

            // Ange spinner-egenskaper
            spinner.Min = 0;
            spinner.Max = 100;
            spinner.IncrementalChange = 5;
            spinner.CurrentValue = 50;

            // Demonstrera Shadow-egenskapen
            spinner.Shadow = true; // Enable 3D shadow effect
            Console.WriteLine("Spinner shadow enabled: " + spinner.Shadow);

            // Spara arbetsboken
            workbook.Save("SpinnerShadowDemo.xlsx");

            // Läs in den sparade arbetsboken för att verifiera skuggningsegenskapen
            Workbook verifyWorkbook = new Workbook("SpinnerShadowDemo.xlsx");
            Spinner verifySpinner = (Spinner)verifyWorkbook.Worksheets[0].Shapes[0];
            Console.WriteLine("Verified spinner shadow: " + verifySpinner.Shadow);
        }
    }
}
```

### Se även

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


