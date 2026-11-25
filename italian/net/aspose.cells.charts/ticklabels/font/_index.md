---
title: "TickLabels.Font"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TickLabels. Restituisce un oggetto Font che rappresenta il carattere dell'oggetto TickLabels specificato"
type: docs
url: /it/net/aspose.cells.charts/ticklabels/font/
---
## TickLabels.Font property

Restituisce un oggetto `Font` che rappresenta il carattere dell'oggetto TickLabels specificato.

```csharp
public Font Font { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyFontDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            
            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.CategoryData = "A1:A1";
            
            // Accedi al carattere delle etichette dei tick
            Aspose.Cells.Charts.TickLabels tickLabels = chart.CategoryAxis.TickLabels;
            Font font = tickLabels.Font;
            
            // Imposta le proprietà del font
            font.Name = "Arial";
            font.Size = 12;
            font.IsBold = true;
            
            // Salva la cartella di lavoro
            workbook.Save("TickLabelsFontDemo.xlsx");
            
            Console.WriteLine("TickLabels font properties set successfully.");
        }
    }
}
```

### Vedi anche

* class [Font](../../../aspose.cells/font/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


