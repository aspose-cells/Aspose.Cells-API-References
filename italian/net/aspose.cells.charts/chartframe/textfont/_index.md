---
title: "ChartFrame.TextFont"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartFrame. Ottiene un oggetto Font dell'oggetto ChartFrame specificato"
type: docs
url: /it/net/aspose.cells.charts/chartframe/textfont/
---
## ChartFrame.TextFont property

Ottiene un oggetto [`Font`](../font/) dell'oggetto ChartFrame specificato.

```csharp
[Obsolete("Use ChartFrame.Font property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual Font TextFont { get; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà ChartFrame.Font. Questa proprietà sarà rimossa 12 mesi dopo, a partire da gennaio 2012. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyTextFontDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Imposta il titolo del grafico e configura il font
            chart.Title.Text = "Sample Chart";
            chart.Title.TextFont.Name = "Arial";
            chart.Title.TextFont.Size = 14;
            chart.Title.TextFont.IsBold = true;
            chart.Title.TextFont.Color = System.Drawing.Color.Blue;

            // Salva la cartella di lavoro
            workbook.Save("ChartTitleFontDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Font](../../../aspose.cells/font/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


