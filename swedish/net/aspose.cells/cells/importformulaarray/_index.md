---
title: "Cells.ImportFormulaArray"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Importerar en matris av formler till ett kalkylblad"
type: docs
url: /sv/net/aspose.cells/cells/importformulaarray/
---
## Cells.ImportFormulaArray method

Importerar en matris av formler till ett kalkylblad.

```csharp
public void ImportFormulaArray(string[] stringArray, int firstRow, int firstColumn, bool isVertical)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stringArray | String[] | Formelmatris. |
| firstRow | Int32 | Radnumret för den första cellen att importera i. |
| firstColumn | Int32 | Kolumnnumret för den första cellen att importera i. |
| ärVertikal | Boolean | Anger om data ska importeras vertikalt eller horisontellt. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportFormulaArrayWithStringInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Förbered formelmatris och parametrar
            string[] formulas = new string[] { "=A1+B1", "=C1*D1" };
            int firstRow = 0;
            int firstColumn = 0;
            bool isVertical = true;

            try
            {
                // Importera formler vertikalt med start i cell A1
                worksheet.Cells.ImportFormulaArray(formulas, firstRow, firstColumn, isVertical);
                
                // Ange värden för formelreferenser
                worksheet.Cells["A1"].PutValue(2);
                worksheet.Cells["B1"].PutValue(3);
                worksheet.Cells["C1"].PutValue(4);
                worksheet.Cells["D1"].PutValue(5);
                
                // Beräkna formler
                workbook.CalculateFormula();

                Console.WriteLine("Formulas imported successfully. Calculated results:");
                Console.WriteLine($"A2 value: {worksheet.Cells["A2"].Value}"); // Should be 5
                Console.WriteLine($"A3 value: {worksheet.Cells["A3"].Value}"); // Should be 20
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportFormulaArray method: {ex.Message}");
            }
            
            // Spara arbetsboken
            workbook.Save("CellsMethodImportFormulaArrayWithStringInt32Int32BooleanDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


