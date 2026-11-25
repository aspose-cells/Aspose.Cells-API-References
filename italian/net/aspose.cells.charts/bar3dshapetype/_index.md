---
title: "Enum Bar3DShapeType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.Bar3DShapeType enum. Rappresenta la forma usata con il grafico a barre o colonne 3D"
type: docs
url: /it/net/aspose.cells.charts/bar3dshapetype/
---
## Bar3DShapeType enumeration

Rappresenta la forma utilizzata con il grafico a barre o colonne 3-D.

```csharp
public enum Bar3DShapeType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Box | `0` | Riquadro |
| PyramidToPoint | `1` | PyramidToPoint |
| PyramidToMax | `2` | PyramidToMax |
| Cylinder | `3` | Cylinder |
| ConeToPoint | `4` | ConeToPoint |
| ConeToMax | `5` | ConeToMax |

### Esempi

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
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();
            // Aggiunta di un nuovo foglio di lavoro all'oggetto Excel
            int sheetIndex = workbook.Worksheets.Add();
            // Ottenere il riferimento del foglio di lavoro appena aggiunto passando il suo indice di foglio
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Aggiunta di valori di esempio alle celle
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

            // Aggiunta di un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column3DClustered, 5, 0, 15, 5);
            // Accesso all'istanza del grafico appena aggiunto
            Chart chart = worksheet.Charts[chartIndex];
            // Aggiunta di NSeries (origine dati del grafico) al grafico che va dalla cella "A1" alla "B4"
            int seriesIndex = chart.NSeries.Add("A1:B4", true);
            // Impostazione dell'origine dati per i dati di categoria di NSeries
            chart.NSeries.CategoryData = "C1:C4";
            Series series = chart.NSeries[seriesIndex];
            // Impostazione dei valori della serie
            series.Values = "=B1:B4";

            // Impostazione del tipo di forma 3D per la serie
            series.Bar3DShapeType = Bar3DShapeType.Cylinder;

            // Salvataggio del file Excel
            workbook.Save("Bar3DShapeTypeExample.xlsx");
            workbook.Save("Bar3DShapeTypeExample.pdf");

            // Impostazione del tipo di forma 3D per la serie
            series.Bar3DShapeType = Bar3DShapeType.ConeToMax;

            // Salvataggio del file Excel
            workbook.Save("Bar3DShapeTypeExample2.xlsx");
            workbook.Save("Bar3DShapeTypeExample2.pdf");
            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


