---
title: "Enum ChartTextDirectionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.ChartTextDirectionType enum. Rappresenta il tipo di direzione del testo del grafico"
type: docs
url: /it/net/aspose.cells.charts/charttextdirectiontype/
---
## ChartTextDirectionType enumeration

Rappresenta il tipo di direzione del testo del grafico.

```csharp
public enum ChartTextDirectionType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Horizontal | `0` | Tipo di direzione orizzontale. |
| Vertical | `1` | Tipo di direzione verticale. |
| Rotate90 | `2` | Ruota di un angolo di novanta gradi. |
| Rotate270 | `3` | Ruota di un angolo di 270 gradi. |
| Stacked | `4` | Testo impilato. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartTextDirectionTypeDemo
    {
        public static void ChartTextDirectionTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi serie di dati al grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Imposta il titolo del grafico
            chart.Title.Text = "Sample Chart";
            chart.Title.Font.Color = Color.Blue;
            
            // Imposta la direzione del testo del titolo del grafico
            chart.Title.DirectionType = ChartTextDirectionType.Rotate90;
            
            // Imposta la direzione del testo del titolo dell'asse delle categorie
            chart.CategoryAxis.Title.Text = "Categories";
            chart.CategoryAxis.Title.DirectionType = ChartTextDirectionType.Vertical;
            
            // Imposta la direzione del testo del titolo dell'asse dei valori
            chart.ValueAxis.Title.Text = "Values";
            chart.ValueAxis.Title.DirectionType = ChartTextDirectionType.Horizontal;
            
            // Salva la cartella di lavoro
            workbook.Save("ChartTextDirectionTypeExample.xlsx");
            workbook.Save("ChartTextDirectionTypeExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


