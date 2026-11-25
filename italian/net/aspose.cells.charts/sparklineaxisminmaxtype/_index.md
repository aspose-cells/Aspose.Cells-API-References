---
title: "Enum SparklineAxisMinMaxType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.SparklineAxisMinMaxType enum. Rappresenta i tipi di valore minimo e massimo per l'asse verticale dello sparkline"
type: docs
url: /it/net/aspose.cells.charts/sparklineaxisminmaxtype/
---
## SparklineAxisMinMaxType enumeration

Rappresenta i tipi di valore minimo e massimo per l'asse verticale dello sparkline.

```csharp
public enum SparklineAxisMinMaxType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| AutoIndividual | `0` | Automatico per ogni sparkline. |
| Group | `1` | Stesso per tutti gli sparkline nel gruppo. |
| Custom | `2` | Valore personalizzato per lo sparkline. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class SparklineAxisMinMaxTypeDemo
    {
        public static void SparklineAxisMinMaxTypeExample()
        {
            // Crea una cartella di lavoro e un foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati al worksheet
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);

            // Definisci il CellArea
            CellArea cellArea = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Aggiungi un gruppo di sparkline al foglio di lavoro
            int sparklineGroupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, cellArea);
            SparklineGroup sparklineGroup = worksheet.SparklineGroups[sparklineGroupIndex];
            sparklineGroup.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

            // Imposta le proprietà per il gruppo di sparkline
            sparklineGroup.VerticalAxisMaxValueType = SparklineAxisMinMaxType.Group;
            sparklineGroup.VerticalAxisMinValueType = SparklineAxisMinMaxType.AutoIndividual;

            // Crea CellsColor
            CellsColor highPointColor = workbook.CreateCellsColor();
            highPointColor.Color = Color.Green;
            sparklineGroup.HighPointColor = highPointColor;

            CellsColor lowPointColor = workbook.CreateCellsColor();
            lowPointColor.Color = Color.Red;
            sparklineGroup.LowPointColor = lowPointColor;

            // Imposta proprietà aggiuntive
            sparklineGroup.ShowHighPoint = true;
            sparklineGroup.ShowLowPoint = true;
            sparklineGroup.LineWeight = 1.0;

            // Salva la cartella di lavoro
            workbook.Save("SparklineAxisMinMaxTypeExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


