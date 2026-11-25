---
title: "ChartCollection.RemoveAt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ChartCollection. Rimuovi un grafico all'indice specificato"
type: docs
url: /it/net/aspose.cells.charts/chartcollection/removeat/
---
## ChartCollection.RemoveAt method

Rimuovi un grafico all'indice specificato.

```csharp
public void RemoveAt(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | L'indice del grafico. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(20);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Mostra il conteggio iniziale dei grafici
            Console.WriteLine("Initial chart count: " + sheet.Charts.Count);

            // Rimuovi il grafico all'indice 0
            sheet.Charts.RemoveAt(0);

            // Mostra il conteggio dei grafici dopo la rimozione
            Console.WriteLine("Chart count after removal: " + sheet.Charts.Count);
        }
    }
}
```

### Vedi anche

* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


