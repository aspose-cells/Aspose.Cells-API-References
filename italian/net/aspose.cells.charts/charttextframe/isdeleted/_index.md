---
title: "ChartTextFrame.IsDeleted"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartTextFrame. Indica se questa etichetta dati è eliminata"
type: docs
url: /it/net/aspose.cells.charts/charttextframe/isdeleted/
---
## ChartTextFrame.IsDeleted property

Indica se questa etichetta dati è eliminata.

```csharp
public bool IsDeleted { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyIsDeletedDemo
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
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accedi alle etichette dati e dimostra la proprietà IsDeleted
            chart.NSeries[0].DataLabels.ShowValue = true;
            bool isDeletedBefore = chart.NSeries[0].DataLabels.IsDeleted;
            
            // Rimuovi le etichette dati impostando ShowValue su false
            chart.NSeries[0].DataLabels.ShowValue = false;
            bool isDeletedAfter = chart.NSeries[0].DataLabels.IsDeleted;

            Console.WriteLine($"DataLabels IsDeleted before removal: {isDeletedBefore}");
            Console.WriteLine($"DataLabels IsDeleted after removal: {isDeletedAfter}");
        }
    }
}
```

### Vedi anche

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


