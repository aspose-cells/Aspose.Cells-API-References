---
title: "Aufzählung PivotTableSelectionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Pivot.PivotTableSelectionType enum. Gibt an, was in einer PivotTable während einer strukturierten Auswahl ausgewählt werden kann. Diese Konstanten können kombiniert werden, um mehrere Typen auszuwählen."
type: docs
url: /de/net/aspose.cells.pivot/pivottableselectiontype/
---
## PivotTableSelectionType enumeration

Gibt an, was in einer PivotTable während einer strukturierten Auswahl ausgewählt werden kann. Diese Konstanten können kombiniert werden, um mehrere Typen auszuwählen.

```csharp
public enum PivotTableSelectionType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| DataAndLabel | `0` | Daten und Beschriftungen |
| DataOnly | `2` | Wählt nur Daten aus |
| LabelOnly | `1` | Wählt nur Beschriftungen aus |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableSelectionTypeDemo
    {
        public static void PivotTableSelectionTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Daten für die PivotTable hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(200);
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B5"].PutValue(250);

            // Erstelle eine PivotTable
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Felder zur PivotTable hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Erstelle einen PivotArea und setze seine Eigenschaften
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.OnlyData = false;
            pivotArea.OnlyLabel = true;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = true;
            pivotArea.IsOutline = false;

            // Wähle den Bereich mit einem bestimmten Auswahltyp aus
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.LabelOnly);

            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableSelectionTypeExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


