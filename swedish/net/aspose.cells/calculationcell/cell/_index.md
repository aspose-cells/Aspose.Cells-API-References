---
title: "CalculationCell.Cell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CalculationCell egenskap. Hämtar Cell-objektet som beräknas"
type: docs
url: /sv/net/aspose.cells/calculationcell/cell/
---
## CalculationCell.Cell property

Hämtar Cell-objektet som beräknas.

```csharp
public Cell Cell { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CalculationCellPropertyCellDemo
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

                // Visa Cell-egenskapens värde
                Console.WriteLine("Cell Name: " + calcCell.Cell.Name);
                Console.WriteLine("Cell Value: " + calcCell.Cell.Value);
                Console.WriteLine("Cell StringValue: " + calcCell.Cell.StringValue);
                Console.WriteLine("Cell Row: " + calcCell.Cell.Row);
                Console.WriteLine("Cell Column: " + calcCell.Cell.Column);
                Console.WriteLine("Cell IsFormula: " + calcCell.Cell.IsFormula);

                // Visa relaterade egenskaper för kontext
                Console.WriteLine("CellRow: " + calcCell.CellRow);
                Console.WriteLine("CellColumn: " + calcCell.CellColumn);

                // Spara arbetsboken
                workbook.Save("CellDemo.xlsx");
                Console.WriteLine("Cell property demonstration completed successfully.");
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

* class [Cell](../../cell/)
* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


