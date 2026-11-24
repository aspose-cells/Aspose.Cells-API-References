---
title: "Klasse PivotTableCalculateOption"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Pivot.PivotTableCalculateOption class. Stellt die Optionen zur Berechnung der Daten der PivotTable dar"
type: docs
url: /de/net/aspose.cells.pivot/pivottablecalculateoption/
---
## PivotTableCalculateOption class

Stellt die Optionen zur Berechnung von Daten der Pivot‑Tabelle dar.

```csharp
public class PivotTableCalculateOption
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [PivotTableCalculateOption](pivottablecalculateoption/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [RefreshCharts](../../aspose.cells.pivot/pivottablecalculateoption/refreshcharts/) { get; set; } | Gibt an, ob Diagramme basierend auf dieser PivotTable aktualisiert werden. |
| [RefreshData](../../aspose.cells.pivot/pivottablecalculateoption/refreshdata/) { get; set; } | Gibt an, ob die Datenquelle der PivotTable aktualisiert wird. |
| [RefreshOption](../../aspose.cells.pivot/pivottablecalculateoption/refreshoption/) { get; set; } | Liest und setzt Optionen für das Aktualisieren der Datenquelle im Pivot-Cache. |
| [ReserveMissingPivotItemType](../../aspose.cells.pivot/pivottablecalculateoption/reservemissingpivotitemtype/) { get; set; } | Stellt dar, wie fehlende Pivot-Elemente reserviert werden. |

### Beispiele

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotTableCalculateOptionDemo
    {
        public static void PivotTableCalculateOptionExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie einige Daten für die Pivot‑Tabelle hinzu
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["B3"].PutValue(30);
            sheet.Cells["A4"].PutValue("Fruit");
            sheet.Cells["B4"].PutValue(70);
            sheet.Cells["A5"].PutValue("Vegetable");
            sheet.Cells["B5"].PutValue(40);

            // Fügen Sie der Arbeitsmappe eine PivotTable hinzu
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // PivotTable konfigurieren
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Amount

            // Ein PivotTableCalculateOption-Objekt erstellen
            PivotTableCalculateOption calculateOption = new PivotTableCalculateOption
            {
                RefreshData = true,
                RefreshCharts = true,
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Berechnen Sie die PivotTable-Daten mit den angegebenen Optionen
            pivotTable.CalculateData(calculateOption);

            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableCalculateOptionExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


