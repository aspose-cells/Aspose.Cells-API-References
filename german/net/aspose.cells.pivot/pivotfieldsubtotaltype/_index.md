---
title: "Enum PivotFieldSubtotalType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Pivot.PivotFieldSubtotalType Enum. Zusammenfassende Beschreibung für PivotFieldSubtotalType"
type: docs
url: /de/net/aspose.cells.pivot/pivotfieldsubtotaltype/
---
## PivotFieldSubtotalType enumeration

Kurzbeschreibung für PivotFieldSubtotalType.

```csharp
[Flags]
public enum PivotFieldSubtotalType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Stellt den Subtotaltyp None dar. |
| Automatic | `1` | Stellt den Subtotaltyp Automatic dar. |
| Sum | `2` | Stellt den Subtotaltyp Sum dar. |
| Count | `4` | Stellt den Subtotaltyp Count dar. |
| Average | `8` | Stellt den Subtotaltyp Average dar. |
| Max | `10` | Stellt den Subtotaltyp Max dar. |
| Min | `20` | Stellt den Subtotaltyp Min dar. |
| Product | `40` | Stellt den Subtotaltyp Product dar. |
| CountNums | `80` | Stellt den Subtotaltyp Count Nums dar. |
| Stdev | `100` | Stellt den Subtotaltyp Standard Deviation dar. |
| Stdevp | `200` | Stellt den Subtotaltyp Standard Deviation of a Population dar. |
| Var | `400` | Stellt den Subtotaltyp Variance dar. |
| Varp | `800` | Stellt den Subtotaltyp Variance of a Population dar. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldSubtotalTypeDemo
    {
        public static void PivotFieldSubtotalTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[3, 0].Value = "Cherry";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[3, 1].Value = 2020;
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 2].Value = 70;

            // Fügen Sie eine Pivot-Tabelle hinzu
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:C4", "E5", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Füge Felder zur Pivot-Tabelle hinzu
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Legen Sie den Subtotaltyp für das Zeilenfeld fest
            PivotField rowField = pivotTable.RowFields[0];
            rowField.SetSubtotals(PivotFieldSubtotalType.Sum, true);
            rowField.SetSubtotals(PivotFieldSubtotalType.Count, true);

            // Aktualisieren und berechnen Sie die Pivot-Tabellendaten
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Speichere die Arbeitsmappe
            workbook.Save("PivotFieldSubtotalTypeExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


