---
title: "SparklineGroup.DisplayHidden"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SparklineGroup. Indica se mostrare i dati in righe e colonne nascoste"
type: docs
url: /it/net/aspose.cells.charts/sparklinegroup/displayhidden/
---
## SparklineGroup.DisplayHidden property

Indica se mostrare i dati in righe e colonne nascoste.

```csharp
public bool DisplayHidden { get; set; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyDisplayHiddenDemo
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

            // Aggiungi la sparkline al gruppo
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Configura l'aspetto dello sparkline
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = Color.Blue;
            group.SeriesColor = seriesColor;

            // Dimostra la proprietà DisplayHidden
            group.DisplayHidden = true; // Show sparklines for hidden data

            // Salva la cartella di lavoro
            workbook.Save("SparklineDisplayHiddenDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


