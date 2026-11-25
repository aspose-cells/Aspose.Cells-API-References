---
title: "SparklineGroup.VerticalAxisMaxValueType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SparklineGroup. Rappresenta il tipo di valore massimo dell'asse verticale"
type: docs
url: /it/net/aspose.cells.charts/sparklinegroup/verticalaxismaxvaluetype/
---
## SparklineGroup.VerticalAxisMaxValueType property

Rappresenta il tipo di valore massimo dell'asse verticale.

```csharp
public SparklineAxisMinMaxType VerticalAxisMaxValueType { get; set; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyVerticalAxisMaxValueTypeDemo
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

            // Configura le impostazioni dell'asse verticale
            group.VerticalAxisMaxValueType = SparklineAxisMinMaxType.Group;
            group.VerticalAxisMaxValue = 10.0;
            group.VerticalAxisMinValueType = SparklineAxisMinMaxType.Custom;
            group.VerticalAxisMinValue = 0.0;

            // Salva la cartella di lavoro
            workbook.Save("SparklineVerticalAxisDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [SparklineAxisMinMaxType](../../sparklineaxisminmaxtype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


