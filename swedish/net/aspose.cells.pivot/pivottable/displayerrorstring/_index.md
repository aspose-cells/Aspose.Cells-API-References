---
title: "PivotTable.DisplayErrorString"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable egenskap. Anger om PivotTable-rapporten visar en anpassad sträng i celler som innehåller fel"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/displayerrorstring/
---
## PivotTable.DisplayErrorString property

Anger om pivottabellsrapporten visar en anpassad sträng i celler som innehåller fel.

```csharp
public bool DisplayErrorString { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDisplayErrorStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Bike";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Car";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Bike";
            cells["B4"].Value = 1500;
            cells["A5"].Value = "Car";
            cells["B5"].Value = 2500;

            // Skapa pivottabell
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Ställ in DisplayErrorString-egenskapen och demonstrera dess användning
            pivotTable.DisplayErrorString = true;
            pivotTable.ErrorString = "Custom Error";

            // Beräkna data för att visa effekten
            pivotTable.CalculateData();

            Console.WriteLine("DisplayErrorString is set to: " + pivotTable.DisplayErrorString);
            Console.WriteLine("ErrorString is set to: " + pivotTable.ErrorString);

            // Spara arbetsboken
            workbook.Save("PivotTablePropertyDisplayErrorStringDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


