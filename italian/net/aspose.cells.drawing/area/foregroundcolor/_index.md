---
title: "Area.ForegroundColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Area. Ottiene o imposta il Color di primo piano"
type: docs
url: /it/net/aspose.cells.drawing/area/foregroundcolor/
---
## Area.ForegroundColor property

Ottiene o imposta il colore di primo piano.

```csharp
public Color ForegroundColor { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AreaPropertyForegroundColorDemo
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

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Imposta colori di primo piano diversi per ogni area della serie
            chart.NSeries[0].Area.ForegroundColor = Color.FromArgb(79, 129, 189);
            chart.NSeries[1].Area.ForegroundColor = Color.FromArgb(192, 80, 77);

            // Salva la cartella di lavoro
            workbook.Save("AreaForegroundColorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


