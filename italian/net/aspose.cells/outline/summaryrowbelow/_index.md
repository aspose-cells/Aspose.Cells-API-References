---
title: "Outline.SummaryRowBelow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Outline. Indica se la riga di riepilogo sarà posizionata sotto le righe di dettaglio nell'outline"
type: docs
url: /it/net/aspose.cells/outline/summaryrowbelow/
---
## Outline.SummaryRowBelow property

Indica se la riga di riepilogo sarà posizionata sotto le righe di dettaglio nella struttura.

```csharp
public bool SummaryRowBelow { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OutlinePropertySummaryRowBelowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio e raggruppamento
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("Total");
            worksheet.Cells["B4"].PutValue("=SUM(B2:B3)");
            
            // Raggruppa le righe e imposta la posizione della riga di riepilogo
            worksheet.Cells.GroupRows(1, 2, false);
            Outline outline = worksheet.Outline;
            outline.SummaryRowBelow = true;
            
            workbook.Save("OutlineSummaryRowBelow.xlsx");
        }
    }
}
```

### Vedi anche

* class [Outline](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


