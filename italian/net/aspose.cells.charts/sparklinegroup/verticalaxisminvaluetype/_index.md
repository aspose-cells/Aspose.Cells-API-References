---
title: "SparklineGroup.VerticalAxisMinValueType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SparklineGroup. Rappresenta il tipo di valore minimo dell'asse verticale"
type: docs
url: /it/net/aspose.cells.charts/sparklinegroup/verticalaxisminvaluetype/
---
## SparklineGroup.VerticalAxisMinValueType property

Rappresenta il tipo di valore minimo dell'asse verticale.

```csharp
public SparklineAxisMinMaxType VerticalAxisMinValueType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyVerticalAxisMinValueTypeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro e un foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);

            // Definisci la posizione dello sparkline
            CellArea cellArea = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Aggiungi gruppo di sparkline
            int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, cellArea);
            SparklineGroup group = worksheet.SparklineGroups[groupIndex];
            group.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

            // Imposta il tipo di valore minimo dell'asse verticale
            group.VerticalAxisMinValueType = SparklineAxisMinMaxType.AutoIndividual;

            // Salva la cartella di lavoro
            workbook.Save("SparklineVerticalAxisMinValueTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [SparklineAxisMinMaxType](../../sparklineaxisminmaxtype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


