---
title: "Enum QuartileCalculationType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.QuartileCalculationType enum. Rappresenta i metodi di calcolo del quartile"
type: docs
url: /it/net/aspose.cells.charts/quartilecalculationtype/
---
## QuartileCalculationType enumeration

Rappresenta i metodi di calcolo del quartile.

```csharp
public enum QuartileCalculationType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Exclusive | `0` | Il calcolo del quartile include la mediana quando si suddivide il set di dati in quartili. |
| Inclusive | `1` | Il calcolo del quartile esclude la mediana quando si suddivide il set di dati in quartili. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class QuartileCalculationTypeDemo
    {
        public static void QuartileCalculationTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["A5"].PutValue("Q4");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.BoxWhisker, 7, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Aggiungi serie al grafico
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Accedi alle proprietà di layout della serie
            SeriesLayoutProperties layoutProperties = chart.NSeries[0].LayoutProperties;

            // Imposta il tipo di calcolo del quartile
            layoutProperties.QuartileCalculation = QuartileCalculationType.Exclusive;

            // Salva la cartella di lavoro
            workbook.Save("QuartileCalculationTypeExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


