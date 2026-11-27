---
title: "CalculationCell.CellRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CalculationCell egenskap. Hämtar radindexet för cellen"
type: docs
url: /sv/net/aspose.cells/calculationcell/cellrow/
---
## CalculationCell.CellRow property

Hämtar radindex för cellen.

```csharp
public int CellRow { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CalculationCellPropertyCellRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["B1"].Formula = "=A1*2";

            try
            {
                // Skapa en CalculationCell-instans med reflektion eftersom konstruktorn är icke-publik
                CalculationCell calcCell = (CalculationCell)Activator.CreateInstance(
                    typeof(CalculationCell),
                    BindingFlags.NonPublic | BindingFlags.Instance,
                    null,
                    new object[] { workbook, worksheet, 0, 1, worksheet.Cells["B1"] },
                    null);

                // Visa CellRow-egenskapens värde
                Console.WriteLine("CellRow value: " + calcCell.CellRow);

                // Visa relaterade egenskaper för kontext
                Console.WriteLine("CellColumn value: " + calcCell.CellColumn);
                Console.WriteLine("Cell Value: " + calcCell.Cell.Value);

                // Spara arbetsboken
                workbook.Save("CellRowDemo.xlsx");
                Console.WriteLine("CellRow property demonstration completed successfully.");
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


