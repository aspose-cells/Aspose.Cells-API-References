---
title: "Enum FormattingType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.FormattingType Aufzählung. Stellt den Typ der Formatierung dar, die auf ein Area-Objekt oder ein Line-Objekt angewendet wird"
type: docs
url: /de/net/aspose.cells.charts/formattingtype/
---
## FormattingType enumeration

Stellt den Typ der Formatierung dar, die auf ein [`Area`](../../aspose.cells.drawing/area/) Objekt oder ein [`Line`](../../aspose.cells.drawing/line/) Objekt angewendet wird.

```csharp
public enum FormattingType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Automatic | `0` | Stellt den automatischen Formatierungstyp dar. |
| Custom | `2` | Stellt den benutzerdefinierten Formatierungstyp dar. |
| None | `1` | Stellt den Formatierungstyp "keine" dar. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class FormattingTypeDemo
    {
        public static void FormattingTypeExample()
        {
            // Instanziiere ein Workbook-Objekt
            Workbook workbook = new Workbook();
            
            // Hinzufügen eines neuen Arbeitsblatts zum Workbook-Objekt
            int sheetIndex = workbook.Worksheets.Add();
            
            // Abrufen der Referenz des neu hinzugefügten Arbeitsblatts durch Übergabe seines Blattindexes
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Hinzufügen von Beispielwerten zu Zellen
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            
            // Hinzufügen eines Diagramms zum Arbeitsblatt
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            
            // Zugriff auf die Instanz des neu hinzugefügten Diagramms
            Chart chart = worksheet.Charts[chartIndex];
            
            // Hinzufügen von NSeries (Diagrammdatenquelle) zum Diagramm im Bereich von "A1"-Zelle bis "B3"
            chart.NSeries.Add("A1:B3", true);
            
            // Festlegen der Vordergrundfarbe des Plotbereichs
            chart.PlotArea.Area.ForegroundColor = Color.Blue;
            chart.PlotArea.Area.Formatting = FormattingType.Custom;
            
            // Festlegen der Vordergrundfarbe des Diagrammbereichs
            chart.ChartArea.Area.ForegroundColor = Color.Yellow;
            chart.ChartArea.Area.Formatting = FormattingType.Automatic;
            
            // Festlegen der Vordergrundfarbe des 1. NSeries-Bereichs
            chart.NSeries[0].Area.ForegroundColor = Color.Red;
            chart.NSeries[0].Area.Formatting = FormattingType.None;
            
            // Festlegen der Vordergrundfarbe des Bereichs des 1. NSeries-Punktes
            chart.NSeries[0].Points[0].Area.ForegroundColor = Color.Cyan;
            chart.NSeries[0].Points[0].Area.Formatting = FormattingType.Custom;
            
            // Die Excel-Datei speichern
            workbook.Save("FormattingTypeExample.xlsx");
            workbook.Save("FormattingTypeExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


