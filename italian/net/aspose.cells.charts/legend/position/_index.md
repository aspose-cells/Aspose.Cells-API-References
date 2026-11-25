---
title: "Legend.Position"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Legend. Ottiene o imposta il tipo di posizione della legenda"
type: docs
url: /it/net/aspose.cells.charts/legend/position/
---
## Legend.Position property

Ottiene o imposta il tipo di posizione della legenda.

```csharp
public LegendPositionType Position { get; set; }
```

### Osservazioni

La posizione predefinita è a destra. Se la legenda è sul lato sinistro o destro del grafico, l'impostazione della proprietà Legend.X non avrà effetto. Se la legenda è sul lato superiore o inferiore del grafico, l'impostazione della proprietà Legend.Y non avrà effetto.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendPropertyPositionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Imposta la posizione della legenda
            chart.Legend.Position = LegendPositionType.Left;

            // Salva la cartella di lavoro
            workbook.Save("LegendPositionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [LegendPositionType](../../legendpositiontype/)
* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


