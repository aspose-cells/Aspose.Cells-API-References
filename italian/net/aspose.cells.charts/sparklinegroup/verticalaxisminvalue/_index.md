---
title: "SparklineGroup.VerticalAxisMinValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SparklineGroup. Ottiene e imposta il valore minimo personalizzato per l'asse verticale"
type: docs
url: /it/net/aspose.cells.charts/sparklinegroup/verticalaxisminvalue/
---
## SparklineGroup.VerticalAxisMinValue property

Ottiene e imposta il valore minimo personalizzato per l'asse verticale.

```csharp
public double VerticalAxisMinValue { get; set; }
```

### Osservazioni

Se questa proprietà è impostata, [`VerticalAxisMinValueType`](../verticalaxisminvaluetype/) sarà Custom.

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyVerticalAxisMinValueDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["A2"].PutValue(2);
            sheet.Cells["A3"].PutValue(1);
            sheet.Cells["A4"].PutValue(3);

            // Crea gruppo sparkline
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 3;
            ca.StartColumn = 4;
            ca.EndColumn = 4;
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:A4", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Imposta valore minimo dell'asse verticale
            group.VerticalAxisMinValueType = SparklineAxisMinMaxType.Custom;
            group.VerticalAxisMinValue = 0.0;

            // Salva la cartella di lavoro
            workbook.Save("SparklineVerticalAxisMinValueDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


