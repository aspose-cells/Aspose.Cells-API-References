---
title: "ListColumn.SetCustomCalculatedFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListColumn-metod. Ställer in formeln för den här listkolumnen"
type: docs
url: /sv/net/aspose.cells.tables/listcolumn/setcustomcalculatedformula/
---
## ListColumn.SetCustomCalculatedFormula method

Ställer in formeln för denna listkolumn.

```csharp
public void SetCustomCalculatedFormula(string formula, bool isR1C1, bool isLocal)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formel | String | formeln för den här listkolumnen. |
| isR1C1 | Boolean | Om formeln behöver formateras som R1C1. |
| isLocal | Boolean | Om formeln behöver formateras enligt lokala inställningar. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListColumnMethodSetCustomCalculatedFormulaWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata för tabellen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["B1"].PutValue("Total");

            // Skapa tabell
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true); // Adjusted parameters to match correct overload
            ListObject table = worksheet.ListObjects[tableIndex];

            // Hämta den andra listkolumnen
            ListColumn totalColumn = table.ListColumns[1];

            try
            {
                // Ange en anpassad formel med A1-notation med standardlokal
                totalColumn.SetCustomCalculatedFormula("=A2*1.1", false, false);
                
                Console.WriteLine("Custom formula set successfully.");
                Console.WriteLine($"Cell B2 formula: {worksheet.Cells["B2"].Formula}");
                Console.WriteLine($"Cell B3 formula: {worksheet.Cells["B3"].Formula}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("SetCustomCalculatedFormulaExample.xlsx");
        }
    }
}
```

### Se även

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


