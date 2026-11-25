---
title: "Outline.SummaryColumnRight"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Outline. Indica se la colonna di riepilogo sarà posizionata a destra delle colonne di dettaglio nell'outline"
type: docs
url: /it/net/aspose.cells/outline/summarycolumnright/
---
## Outline.SummaryColumnRight property

Indica se la colonna di riepilogo sarà posizionata a destra delle colonne di dettaglio nella struttura.

```csharp
public bool SummaryColumnRight { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OutlinePropertySummaryColumnRightDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio e raggruppa le righe
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Item " + (i + 1));
                worksheet.Cells["B" + (i + 1)].PutValue(i * 10);
            }

            // Raggruppa le righe (crea un outline)
            worksheet.Cells.GroupRows(0, 9, false);

            // Ottieni le impostazioni dell'outline
            Outline outline = worksheet.Outline;

            // Imposta SummaryColumnRight su true (le colonne di riepilogo appariranno a destra delle colonne di dettaglio)
            outline.SummaryColumnRight = true;
            Console.WriteLine("SummaryColumnRight is set to: " + outline.SummaryColumnRight);

            // Salva la cartella di lavoro
            workbook.Save("OutlinePropertySummaryColumnRightDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Outline](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


