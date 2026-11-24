---
title: "Klasse PivotTableRefreshOption"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Pivot.PivotTableRefreshOption Klasse. Stellt die Optionen zum Aktualisieren der Datenquelle der Pivot-Tabelle dar."
type: docs
url: /de/net/aspose.cells.pivot/pivottablerefreshoption/
---
## PivotTableRefreshOption class

Stellt die Optionen zum Aktualisieren der Datenquelle der Pivot‑Tabelle dar.

```csharp
public class PivotTableRefreshOption
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [PivotTableRefreshOption](pivottablerefreshoption/)() | Stellt die Optionen zum Aktualisieren der Datenquelle der Pivot‑Tabelle dar. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [IsKeepOriginalOrder](../../aspose.cells.pivot/pivottablerefreshoption/iskeeporiginalorder/) { get; set; } | Gibt an, ob die ursprüngliche Reihenfolge der Pivot-Elemente wie in der alten Datenquelle beibehalten werden soll. |
| [KeepCachedLocalGroupData](../../aspose.cells.pivot/pivottablerefreshoption/keepcachedlocalgroupdata/) { get; set; } | Gibt an, ob zwischengespeicherte lokale Gruppendaten beibehalten werden sollen, wenn die maximalen und minimalen Werte unverändert bleiben. Der Standardwert ist false, was bedeutet, dass die Gruppe mit lokaler Einstellung aktualisiert wird. |
| [ReserveMissingPivotItemType](../../aspose.cells.pivot/pivottablerefreshoption/reservemissingpivotitemtype/) { get; set; } | Stellt dar, wie fehlende Pivot-Elemente reserviert werden. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableRefreshOptionDemo
    {
        public static void PivotTableRefreshOptionExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt einige Daten hinzu
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 0].Value = "Apple";
            worksheet.Cells[3, 1].Value = 2021;
            worksheet.Cells[3, 2].Value = 70;
            worksheet.Cells[4, 0].Value = "Banana";
            worksheet.Cells[4, 1].Value = 2021;
            worksheet.Cells[4, 2].Value = 80;

            // Fügen Sie der Arbeitsmappe eine PivotTable hinzu
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Füge Felder zur Pivot-Tabelle hinzu
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Erstelle eine Instanz von PivotTableRefreshOption
            PivotTableRefreshOption refreshOption = new PivotTableRefreshOption
            {
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Aktualisiere die Pivot-Tabelle mit den angegebenen Optionen
            pivotTable.RefreshData(refreshOption);
            pivotTable.CalculateData();

            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableRefreshOptionExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


