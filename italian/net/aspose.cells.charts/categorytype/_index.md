---
title: "Enum CategoryType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.CategoryType enum. Rappresenta il tipo di asse di categoria"
type: docs
url: /it/net/aspose.cells.charts/categorytype/
---
## CategoryType enumeration

Rappresenta il tipo di asse delle categorie.

```csharp
public enum CategoryType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| AutomaticScale | `0` | AutomaticScale |
| CategoryScale | `1` | CategoryScale |
| TimeScale | `2` | TimeScale |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class CategoryTypeDemo
    {
        public static void CategoryTypeExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();
            // Aggiunta di un nuovo foglio di lavoro all'oggetto Excel
            int sheetIndex = workbook.Worksheets.Add();
            // Ottenere il riferimento del foglio di lavoro appena aggiunto passando il suo indice di foglio
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Aggiunta di valori di esempio alle celle
            worksheet.Cells["A1"].PutValue("Dates");
            worksheet.Cells["A2"].PutValue(new DateOnly(2024, 01, 01));
            worksheet.Cells["A3"].PutValue(new DateOnly(2024, 03, 01));
            worksheet.Cells["A4"].PutValue(new DateOnly(2024, 05, 01));
            worksheet.Cells["B1"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(50);
            worksheet.Cells["C1"].PutValue("Data2");
            worksheet.Cells["C2"].PutValue(8);
            worksheet.Cells["C3"].PutValue(15);
            worksheet.Cells["C4"].PutValue(30);

            // Aggiunta di un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            // Accesso all'istanza del grafico appena aggiunto
            Chart chart = worksheet.Charts[chartIndex];
            // Aggiunta di NSeries (origine dati del grafico) al grafico dall'intervallo di celle "A1" a "B3"
            chart.NSeries.Add("B2:C4", true);

            // Impostazione dei nomi di categoria per l'asse X dall'intervallo "A2:A5"
            chart.NSeries[0].XValues = "A2:A4";

            // Impostazione del tipo di asse di categoria su TimeScale
            chart.CategoryAxis.CategoryType = CategoryType.CategoryScale;

            // Impostazione della scala dell'unità principale per l'asse di categoria
            chart.CategoryAxis.MajorUnitScale = TimeUnit.Months;
            chart.CategoryAxis.MajorUnit = 2;

            // Impostazione della scala dell'unità secondaria per l'asse di categoria
            chart.CategoryAxis.MinorUnitScale = TimeUnit.Months;
            chart.CategoryAxis.MinorUnit = 2;

            // Salvataggio del file Excel
            workbook.Save("CategoryTypeExample.xlsx");
            workbook.Save("CategoryTypeExample.pdf");

        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


