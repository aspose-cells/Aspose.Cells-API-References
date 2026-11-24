---
title: "Enum CrossType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.CrossType enum. Stellt den Achsenkreuzungstyp dar"
type: docs
url: /de/net/aspose.cells.charts/crosstype/
---
## CrossType enumeration

Stellt den Achsenkreuztyp dar.

```csharp
public enum CrossType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Automatic | `0` | Microsoft Excel legt den Achsenkreuzungspunkt fest. |
| Maximum | `1` | Die Achse kreuzt beim Maximalwert. |
| Minimum | `2` | Die Achse kreuzt beim Minimalwert. |
| Custom | `3` | Die Achse kreuzt beim benutzerdefinierten Wert. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class CrossTypeDemo
    {
        public static void CrossTypeExample()
        {
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();
            // Ein neues Arbeitsblatt zum Excel-Objekt hinzufügen
            int sheetIndex = workbook.Worksheets.Add();
            // Abrufen der Referenz des neu hinzugefügten Arbeitsblatts durch Übergabe seines Blattindexes
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Hinzufügen von Beispielwerten zu Zellen
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Hinzufügen eines Diagramms zum Arbeitsblatt
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            // Zugriff auf die Instanz des neu hinzugefügten Diagramms
            Chart chart = worksheet.Charts[chartIndex];
            // Hinzufügen von NSeries (Diagrammdatenquelle) zum Diagramm im Bereich von "A1"-Zelle bis "B3"
            chart.NSeries.Add("A1:B3", true);

            // Legen Sie den Maximalwert der Werteachse fest
            chart.ValueAxis.MaxValue = 200;
            // Legen Sie den Minimalwert der Werteachse fest
            chart.ValueAxis.MinValue = 0;
            // Legen Sie die Haupteinheit fest
            chart.ValueAxis.MajorUnit = 25;

            // Die Kategorie(X)-Achse kreuzt beim Maximalwert
            chart.ValueAxis.CrossType = CrossType.Maximum;

            // Legen Sie die Anzahl der Kategorien oder Serien zwischen den Achsenbeschriftungen fest
            chart.CategoryAxis.TickLabelSpacing = 2;

            // Die Excel-Datei speichern
            workbook.Save("CrossTypeExample.xlsx");
            workbook.Save("CrossTypeExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


