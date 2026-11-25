---
title: "Enum DataLabelsSeparatorType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.DataLabelsSeparatorType enum. Rappresenta il tipo di separatore delle DataLabels"
type: docs
url: /it/net/aspose.cells.charts/datalabelsseparatortype/
---
## DataLabelsSeparatorType enumeration

Rappresenta il tipo di separatore delle etichette dati.

```csharp
public enum DataLabelsSeparatorType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Auto | `0` | Rappresenta il separatore automatico |
| Space | `1` | Rappresenta lo spazio(" ") |
| Comma | `2` | Rappresenta la virgola(",") |
| Semicolon | `3` | Rappresenta il punto e virgola(";") |
| Period | `4` | Rappresenta il punto(".") |
| NewLine | `5` | Rappresenta l'interruzione di riga("\n") |
| Custom | `6` | Rappresenta un separatore personalizzato |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class DataLabelsSeparatorTypeDemo
    {
        public static void DataLabelsSeparatorTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati per il grafico
            worksheet.Cells[0, 0].PutValue("Category");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);
            worksheet.Cells[3, 0].PutValue("C");
            worksheet.Cells[3, 1].PutValue(30);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Aggiungi la serie di dati al grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accedi alle etichette dati della prima serie
            DataLabels dataLabels = chart.NSeries[0].DataLabels;

            // Imposta il tipo di separatore su virgola
            dataLabels.SeparatorType = DataLabelsSeparatorType.Comma;

            // Abilita le etichette dei dati e imposta alcune proprietà
            dataLabels.ShowCategoryName = true;
            dataLabels.ShowValue = true;
            dataLabels.Position = LabelPositionType.InsideBase;

            // Imposta le proprietà del font
            dataLabels.Font.Color = Color.Blue;
            dataLabels.Font.IsBold = true;

            // Salva la cartella di lavoro
            workbook.Save("DataLabelsSeparatorTypeExample.xlsx");
            workbook.Save("DataLabelsSeparatorTypeExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


