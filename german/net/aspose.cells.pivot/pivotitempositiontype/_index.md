---
title: "Aufzählung PivotItemPositionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Pivot.PivotItemPositionType Aufzählung. Stellt den Positionstyp des Pivot-Basis‑Elements im Basisfeld dar, wenn die ShowDataAs‑Berechnung verwendet wird."
type: docs
url: /de/net/aspose.cells.pivot/pivotitempositiontype/
---
## PivotItemPositionType enumeration

Stellt den Positionstyp des Pivot‑Basiselements im Basisfeld dar, wenn die ShowDataAs‑Berechnung verwendet wird.

```csharp
public enum PivotItemPositionType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Previous | `0` | Stellt das vorherige Pivot-Element im PivotField dar. |
| Next | `1` | Stellt das nächste Pivot-Element im PivotField dar. |
| Custom | `2` | Zeigt Werte im unterschiedlichen Format basierend auf dem Index des Pivot-Elements im PivotField an. |

### Beispiele

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotItemPositionTypeDemo
    {
        public static void PivotItemPositionTypeExample()
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

            // Fügen Sie der Arbeitsmappe eine PivotTable hinzu
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Füge Felder zur Pivot-Tabelle hinzu
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Value

            // Setze das Anzeigeformat der Daten, um Werte als Unterschied zum vorherigen Element anzuzeigen
            PivotField dataField = pivotTable.DataFields[0];
            dataField.ShowValuesAs(PivotFieldDataDisplayFormat.DifferenceFrom, 0, PivotItemPositionType.Previous, 0);

            // Aktualisiere und berechne die Pivot-Tabelle
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Speichere die Arbeitsmappe
            workbook.Save("PivotItemPositionTypeExample.xlsx");

            Console.WriteLine("Pivot table created and saved successfully.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


