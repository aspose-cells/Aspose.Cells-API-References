---
title: "Cells.ImportFormulaArray"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Importiert ein Array von Formeln in ein Arbeitsblatt"
type: docs
url: /de/net/aspose.cells/cells/importformulaarray/
---
## Cells.ImportFormulaArray method

Importiert ein Array von Formeln in ein Arbeitsblatt.

```csharp
public void ImportFormulaArray(string[] stringArray, int firstRow, int firstColumn, bool isVertical)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stringArray | String[] | Formel-Array. |
| firstRow | Int32 | Die Zeilennummer der ersten Zelle, in die importiert werden soll. |
| firstColumn | Int32 | Die Spaltennummer der ersten Zelle, in die importiert werden soll. |
| isVertical | Boolean | Gibt an, ob Daten vertikal oder horizontal importiert werden sollen. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportFormulaArrayWithStringInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Formel-Array und Parameter vorbereiten
            string[] formulas = new string[] { "=A1+B1", "=C1*D1" };
            int firstRow = 0;
            int firstColumn = 0;
            bool isVertical = true;

            try
            {
                // Formeln vertikal ab Zelle A1 importieren
                worksheet.Cells.ImportFormulaArray(formulas, firstRow, firstColumn, isVertical);
                
                // Werte für Formelreferenzen festlegen
                worksheet.Cells["A1"].PutValue(2);
                worksheet.Cells["B1"].PutValue(3);
                worksheet.Cells["C1"].PutValue(4);
                worksheet.Cells["D1"].PutValue(5);
                
                // Formeln berechnen
                workbook.CalculateFormula();

                Console.WriteLine("Formulas imported successfully. Calculated results:");
                Console.WriteLine($"A2 value: {worksheet.Cells["A2"].Value}"); // Should be 5
                Console.WriteLine($"A3 value: {worksheet.Cells["A3"].Value}"); // Should be 20
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportFormulaArray method: {ex.Message}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("CellsMethodImportFormulaArrayWithStringInt32Int32BooleanDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


