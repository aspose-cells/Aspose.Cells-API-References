---
title: "CalculationCell.Workbook"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CalculationCell egenskap. Hämtar Workbook-objektet"
type: docs
url: /sv/net/aspose.cells/calculationcell/workbook/
---
## CalculationCell.Workbook property

Hämtar Workbook-objektet.

```csharp
public Workbook Workbook { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CalculationCellPropertyWorkbookDemo
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

                // Visa Workbook-egenskapens värde
                Console.WriteLine("Workbook Name: " + calcCell.Workbook.FileName);
                Console.WriteLine("Workbook Has Macro: " + calcCell.Workbook.HasMacro);
                Console.WriteLine("Workbook Worksheet Count: " + calcCell.Workbook.Worksheets.Count);

                // Visa relaterade egenskaper för kontext
                Console.WriteLine("Worksheet Name: " + calcCell.Worksheet.Name);
                Console.WriteLine("Cell Row: " + calcCell.CellRow);
                Console.WriteLine("Cell Column: " + calcCell.CellColumn);

                // Spara arbetsboken
                workbook.Save("WorkbookDemo.xlsx");
                Console.WriteLine("Workbook property demonstration completed successfully.");
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

* class [Workbook](../../workbook/)
* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


