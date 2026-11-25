---
title: "SparklineGroup.ShowMarkers"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "SparklineGroup proprietà. Indica se evidenziare ogni punto in ogni sparkline di linea nel gruppo sparkline."
type: docs
url: /it/net/aspose.cells.charts/sparklinegroup/showmarkers/
---
## SparklineGroup.ShowMarkers property

Indica se evidenziare ogni punto in ogni sparkline a linea nel gruppo di sparkline.

```csharp
public bool ShowMarkers { get; set; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyShowMarkersDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Definisci la posizione dello sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Aggiungi gruppo di sparkline
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Aggiungi sparkline
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Configura l'aspetto dello sparkline
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = Color.Orange;
            group.SeriesColor = seriesColor;

            group.ShowMarkers = true;
            
            CellsColor markersColor = workbook.CreateCellsColor();
            markersColor.Color = Color.Black;
            group.MarkersColor = markersColor;

            // Salva la cartella di lavoro
            workbook.Save("SparklineWithMarkers.xlsx");
        }
    }
}
```

### Vedi anche

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


