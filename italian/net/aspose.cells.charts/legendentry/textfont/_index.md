---
title: "LegendEntry.TextFont"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LegendEntry. Restituisce un oggetto Font dell'oggetto LegendEntry specificato"
type: docs
url: /it/net/aspose.cells.charts/legendentry/textfont/
---
## LegendEntry.TextFont property

Restituisce un oggetto [`Font`](../font/) dell'oggetto LegendEntry specificato.

```csharp
[Obsolete("Use LegendEntry.Font property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual Font TextFont { get; }
```

### Osservazioni

NOTE: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà LegendEntry.Font. Questa proprietà sarà rimossa 12 mesi dopo, a partire da GENNAIO 2012. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LegendEntryPropertyTextFontDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["B1"].PutValue("Series 2");
            worksheet.Cells["B2"].PutValue(25);
            worksheet.Cells["B3"].PutValue(35);
            worksheet.Cells["B4"].PutValue(45);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A1:B1";

            // Abilita legenda
            chart.ShowLegend = true;
            Legend legend = chart.Legend;

            // Accedi alla prima voce della legenda e modifica le sue proprietà TextFont
            LegendEntry legendEntry = legend.LegendEntries[0];
            Aspose.Cells.Font font = legendEntry.TextFont;
            
            // Imposta varie proprietà del carattere
            font.Name = "Arial";
            font.Size = 12;
            font.Color = Color.Red;
            font.IsBold = true;
            font.IsItalic = true;
            font.Underline = FontUnderlineType.Single;

            // Salva la cartella di lavoro
            workbook.Save("LegendEntryTextFontDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Font](../../../aspose.cells/font/)
* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


