---
title: "Enum TimeUnit"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Charts.TimeUnit. Rappresenta l'unità di base per l'asse delle categorie"
type: docs
url: /it/net/aspose.cells.charts/timeunit/
---
## TimeUnit enumeration

Rappresenta l'unità di base per l'asse delle categorie.

```csharp
public enum TimeUnit
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Days | `0` | Giorni |
| Months | `1` | Mesi |
| Years | `2` | Anni |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TimeUnitDemo
    {
        public static void TimeUnitExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            // Aggiungi un nuovo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["B1"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["B3"].PutValue(300);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Aggiungi serie al grafico
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Imposta l'asse delle categorie per utilizzare unità di tempo
            Axis categoryAxis = chart.CategoryAxis;
            categoryAxis.CategoryType = CategoryType.TimeScale;
            categoryAxis.BaseUnitScale = TimeUnit.Months;
            categoryAxis.MajorUnitScale = TimeUnit.Months;
            categoryAxis.MinorUnitScale = TimeUnit.Days;

            // Personalizza l'aspetto del grafico
            chart.Title.Text = "Sample Chart with Time Units";
            chart.ValueAxis.Title.Text = "Values";
            chart.CategoryAxis.Title.Text = "Dates";

            // Salva la cartella di lavoro
            workbook.Save("TimeUnitExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


