---
title: "ChartArea.Font"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartArea. Ottiene un oggetto Font dell'oggetto ChartArea specificato"
type: docs
url: /it/net/aspose.cells.charts/chartarea/font/
---
## ChartArea.Font property

Ottiene un oggetto `Font` dell'oggetto ChartArea specificato.

```csharp
public override Font Font { get; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartAreaPropertyFontDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Region");
            worksheet.Cells["A2"].PutValue("North");
            worksheet.Cells["A3"].PutValue("South");
            worksheet.Cells["A4"].PutValue("East");
            worksheet.Cells["A5"].PutValue("West");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(5000);
            worksheet.Cells["B3"].PutValue(3000);
            worksheet.Cells["B4"].PutValue(4000);
            worksheet.Cells["B5"].PutValue(6000);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Ottieni l'area del grafico
            ChartArea chartArea = chart.ChartArea;
            
            // Imposta le proprietà del carattere dell'area del grafico
            Aspose.Cells.Font font = chartArea.Font;
            font.Name = "Tahoma";
            font.Size = 10;
            font.Color = Color.Blue;
            font.IsBold = true;
            font.IsItalic = true;
            font.Underline = FontUnderlineType.Single;

            // Salva la cartella di lavoro
            workbook.Save("ChartAreaFontDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Font](../../../aspose.cells/font/)
* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


