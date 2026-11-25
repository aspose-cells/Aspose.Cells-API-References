---
title: "Series.Bar3DShapeType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Ottiene o imposta il tipo di forma 3D utilizzato con il grafico a barre o colonne 3D"
type: docs
url: /it/net/aspose.cells.charts/series/bar3dshapetype/
---
## Series.Bar3DShapeType property

Ottiene o imposta il tipo di forma 3D utilizzato con il grafico a barre o colonne 3D.

```csharp
public Bar3DShapeType Bar3DShapeType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyBar3DShapeTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico a barre 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Imposta il tipo di forma della barra su Cilindro
            chart.NSeries[0].Bar3DShapeType = Bar3DShapeType.Cylinder;

            // Salva la cartella di lavoro
            workbook.Save("Bar3DShapeTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* enum [Bar3DShapeType](../../bar3dshapetype/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


