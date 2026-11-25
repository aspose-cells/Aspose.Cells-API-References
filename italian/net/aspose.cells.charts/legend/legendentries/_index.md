---
title: "Legend.LegendEntries"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Legend. Ottiene una raccolta di tutti gli oggetti LegendEntry nella legenda del grafico specificato. La impostazione delle voci della legenda del grafico a superficie non è supportata. Pertanto restituirà null se il tipo di grafico è di tipo superficie."
type: docs
url: /it/net/aspose.cells.charts/legend/legendentries/
---
## Legend.LegendEntries property

Ottiene una raccolta di tutti gli oggetti LegendEntry nella legenda del grafico specificato. L'impostazione delle voci della legenda per i grafici di superficie non è supportata. Quindi restituirà null se il tipo di grafico è di tipo superficie.

```csharp
public LegendEntryCollection LegendEntries { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendPropertyLegendEntriesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
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
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.CategoryData = "B2:B4";

            // Accedi alle voci della legenda
            Aspose.Cells.Charts.LegendEntryCollection legendEntries = chart.Legend.LegendEntries;
            
            // Elimina la seconda voce della legenda
            legendEntries[1].IsDeleted = true;
            
            // Salva la cartella di lavoro
            workbook.Save("LegendEntriesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [LegendEntryCollection](../../legendentrycollection/)
* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


