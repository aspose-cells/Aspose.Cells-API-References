---
title: "CalculationCell.CellColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CalculationCell egenskap. Hämtar kolumnindexet för cellen"
type: docs
url: /sv/net/aspose.cells/calculationcell/cellcolumn/
---
## CalculationCell.CellColumn property

Hämtar kolumnindex för cellen.

```csharp
public int CellColumn { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationCellPropertyCellColumnDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg in lite data och en enkel formel
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["B1"].Formula = "=A1*2";

            try
            {
                // Skaffa en CalculationCell-instans via reflektion (dess konstruktor är icke‑publik)
                CalculationCell calcCell = (CalculationCell)Activator.CreateInstance(
                    typeof(CalculationCell), 
                    nonPublic: true);

                // Läs och visa värdet för egenskapen CellColumn
                Console.WriteLine("CellColumn value: " + calcCell.CellColumn);

                // Ytterligare demonstration av relaterade egenskaper (valfritt)
                Console.WriteLine("CellRow value: " + calcCell.CellRow);
                Console.WriteLine("Workbook is null: " + (calcCell.Workbook == null));
                Console.WriteLine("Worksheet is null: " + (calcCell.Worksheet == null));

                // Spara arbetsboken (filen kommer att innehålla de data vi lade till)
                workbook.Save("CellColumnDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


