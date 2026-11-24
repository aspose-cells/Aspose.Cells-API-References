---
title: "Enum ConsolidationFunction"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ConsolidationFunction enum. Stellt die Konsolidierungsfunktion dar."
type: docs
url: /de/net/aspose.cells/consolidationfunction/
---
## ConsolidationFunction enumeration

Stellt die Konsolidierungsfunktion dar.

```csharp
public enum ConsolidationFunction
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Sum | `0` | Stellt die Summenfunktion dar. |
| Count | `1` | Stellt die Zählfunktion dar. |
| Average | `2` | Stellt die Mittelwertfunktion dar. |
| Max | `3` | Stellt die Maximalfunktion dar. |
| Min | `4` | Stellt die Minimalfunktion dar. |
| Product | `5` | Stellt die Produktfunktion dar. |
| CountNums | `6` | Stellt die Count Nums‑Funktion dar. |
| StdDev | `7` | Stellt die StdDev‑Funktion dar. |
| StdDevp | `8` | Stellt die StdDevp‑Funktion dar. |
| Var | `9` | Stellt die Var‑Funktion dar. |
| Varp | `10` | Stellt die Varp‑Funktion dar. |
| DistinctCount | `11` | Stellt die Distinct Count‑Funktion dar. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConsolidationFunctionDemo
    {
        public static void ConsolidationFunctionExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Definieren Sie den Zellbereich für die Zwischensumme
            CellArea cellArea = new CellArea
            {
                StartRow = 1,
                StartColumn = 0,
                EndRow = 3,
                EndColumn = 1
            };

            // Zwischensumme mit der Summenfunktion anwenden
            worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Sum, new int[] { 1 });

            // Zwischensumme mit der Mittelwertfunktion anwenden
            worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Average, new int[] { 1 });

            // Zwischensumme mit der Maximalfunktion anwenden
            worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Max, new int[] { 1 });

            // Zwischensumme mit der Minimalfunktion anwenden
            worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Min, new int[] { 1 });

            // Speichere die Arbeitsmappe
            workbook.Save("ConsolidationFunctionExample.xlsx");
            workbook.Save("ConsolidationFunctionExample.pdf");

            // Ergebnisse ausgeben
            Console.WriteLine("Workbook saved with subtotals applied.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


