---
title: "Chart.SubTitle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. Ottiene il sottotitolo del grafico. Valido solo per file ODS"
type: docs
url: /it/net/aspose.cells.charts/chart/subtitle/
---
## Chart.SubTitle property

Ottiene il sottotitolo del grafico. Si applica solo ai file ODS.

```csharp
public Title SubTitle { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertySubTitleDemo
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

            // Aggiungi un grafico e imposta il suo intervallo di dati
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Imposta il titolo principale
            chart.Title.Text = "Main Chart Title";

            // Imposta il sottotitolo
            chart.SubTitle.Text = "Chart Subtitle";
            chart.SubTitle.Font.Size = 12;
            chart.SubTitle.Font.IsBold = true;

            // Salva la cartella di lavoro
            workbook.Save("ChartWithSubtitle.xlsx");
        }
    }
}
```

### Vedi anche

* class [Title](../../title/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


