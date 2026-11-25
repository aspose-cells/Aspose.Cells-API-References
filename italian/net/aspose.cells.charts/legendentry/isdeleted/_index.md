---
title: "LegendEntry.IsDeleted"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LegendEntry. Ottiene e imposta se la voce della legenda è eliminata"
type: docs
url: /it/net/aspose.cells.charts/legendentry/isdeleted/
---
## LegendEntry.IsDeleted property

Ottiene e imposta se la voce di legenda è eliminata.

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
    public class LegendEntryPropertyIsDeletedDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Ottieni la prima voce della legenda
            LegendEntry legendEntry = chart.Legend.LegendEntries[0];

            // Dimostra la proprietà IsDeleted
            Console.WriteLine("Legend entry initially deleted? " + legendEntry.IsDeleted);
            
            // Elimina la voce della legenda
            legendEntry.IsDeleted = true;
            Console.WriteLine("Legend entry after deletion? " + legendEntry.IsDeleted);

            // Ripristina la voce della legenda
            legendEntry.IsDeleted = false;
            Console.WriteLine("Legend entry after restoration? " + legendEntry.IsDeleted);

            // Salva la cartella di lavoro
            workbook.Save("LegendEntryIsDeletedDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


