---
title: "FormulaSettings.PrecisionAsDisplayed"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FormulaSettings-egenskap. Anger om precisionen för beräknat resultat ska sättas som de visas vid beräkning av formler"
type: docs
url: /sv/net/aspose.cells/formulasettings/precisionasdisplayed/
---
## FormulaSettings.PrecisionAsDisplayed property

Anger om precisionen för beräknat resultat ska sättas som de visas under beräkning av formler.

```csharp
public bool PrecisionAsDisplayed { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyPrecisionAsDisplayedDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Ställ in PrecisionAsDisplayed till true
            workbook.Settings.FormulaSettings.PrecisionAsDisplayed = true;
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Ställ in visningsformat för cell A1 för att visa 2 decimaler
            cells["A1"].PutValue(1.23456);
            Style style = cells["A1"].GetStyle();
            style.Number = 2; // Format: 0.00
            cells["A1"].SetStyle(style);
            
            // Ställ in formel i B1 som refererar till A1
            cells["B1"].Formula = "=A1";
            
            // Beräkna formler med PrecisionAsDisplayed aktiverat
            workbook.CalculateFormula();
            
            // Skriv ut resultat
            Console.WriteLine("A1 Display Value: " + cells["A1"].StringValue); // Shows 1.23
            Console.WriteLine("B1 Calculated Value: " + cells["B1"].Value);   // Should be 1.23 due to PrecisionAsDisplayed
        }
    }
}
```

### Se även

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


