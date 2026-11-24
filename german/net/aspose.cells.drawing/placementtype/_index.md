---
title: "Enum PlacementType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.PlacementType Enum. Gibt an, wie das Zeichenobjekt an den darunterliegenden Zellen befestigt ist"
type: docs
url: /de/net/aspose.cells.drawing/placementtype/
---
## PlacementType enumeration

Stellt die Art und Weise dar, wie das Zeichenobjekt an den darunter liegenden Zellen befestigt ist.

```csharp
public enum PlacementType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| FreeFloating | `0` | Nicht mit Zellen verschieben oder skalieren. |
| Move | `1` | Verschieben, aber nicht mit Zellen skalieren. |
| MoveAndSize | `2` | Verschieben und mit Zellen skalieren. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class PlacementTypeDemo
    {
        public static void PlacementTypeExample()
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

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Lege den Datenbereich des Diagramms fest
            chart.SetChartDataRange("A1:B4", true);

            // Lege den Platzierungstyp des Diagramms fest.
            chart.Placement = PlacementType.MoveAndSize;

            // Gib den Platzierungstyp aus.
            Console.WriteLine("Chart Placement Type: " + chart.Placement);

            // Speichere die Arbeitsmappe
            workbook.Save("PlacementTypeExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


