---
title: "ChartFrame.Font"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartFrame. Ottiene un oggetto Font dell'oggetto ChartFrame specificato"
type: docs
url: /it/net/aspose.cells.charts/chartframe/font/
---
## ChartFrame.Font property

Restituisce un oggetto `Font` dell'oggetto ChartFrame specificato.

```csharp
public virtual Font Font { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyFontDemo
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
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Imposta il titolo del grafico e configura le proprietà del font
            chart.Title.Text = "Sample Chart";
            chart.Title.Font.Name = "Arial";
            chart.Title.Font.Size = 14;
            chart.Title.Font.Color = System.Drawing.Color.Blue;
            chart.Title.Font.CapsType = TextCapsType.None;
            chart.Title.Font.IsBold = true;

            // Salva la cartella di lavoro
            workbook.Save("ChartFontDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Font](../../../aspose.cells/font/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


