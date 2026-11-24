---
title: "Enum Bar3DShapeType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.Bar3DShapeType-Enum. Stellt die Form dar, die bei einem 3D-Balken- oder Säulendiagramm verwendet wird"
type: docs
url: /de/net/aspose.cells.charts/bar3dshapetype/
---
## Bar3DShapeType enumeration

Stellt die Form dar, die mit dem 3‑D‑Balken‑ oder Säulendiagramm verwendet wird.

```csharp
public enum Bar3DShapeType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Box | `0` | Box |
| PyramidToPoint | `1` | PyramidToPoint |
| PyramidToMax | `2` | PyramidToMax |
| Cylinder | `3` | Cylinder |
| ConeToPoint | `4` | ConeToPoint |
| ConeToMax | `5` | ConeToMax |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class Bar3DShapeTypeDemo
    {
        public static void Bar3DShapeTypeExample()
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
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Hinzufügen eines Diagramms zum Arbeitsblatt
            int chartIndex = worksheet.Charts.Add(ChartType.Column3DClustered, 5, 0, 15, 5);
            // Zugriff auf die Instanz des neu hinzugefügten Diagramms
            Chart chart = worksheet.Charts[chartIndex];
            // Hinzufügen von NSeries (Diagrammdatenquelle) zum Diagramm vom Feld "A1" bis "B4"
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            // Festlegen der Datenquelle für die Kategoriedaten von NSeries
            chart.NSeries.CategoryData = "C1:C4";
            Series series = chart.NSeries[seriesIndex];
            // Festlegen der Werte der Serie
            series.Values = "=B1:B4";

            // Festlegen des 3D-Formtyps für die Serie
            series.Bar3DShapeType = Bar3DShapeType.Cylinder;

            // Die Excel-Datei speichern
            workbook.Save("Bar3DShapeTypeExample.xlsx");
            workbook.Save("Bar3DShapeTypeExample.pdf");

            // Festlegen des 3D-Formtyps für die Serie
            series.Bar3DShapeType = Bar3DShapeType.ConeToMax;

            // Die Excel-Datei speichern
            workbook.Save("Bar3DShapeTypeExample2.xlsx");
            workbook.Save("Bar3DShapeTypeExample2.pdf");
            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


