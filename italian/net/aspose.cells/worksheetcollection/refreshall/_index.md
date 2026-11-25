---
title: "WorksheetCollection.RefreshAll"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo WorksheetCollection. Aggiorna tutte le tabelle pivot e i grafici con l'origine pivot"
type: docs
url: /it/net/aspose.cells/worksheetcollection/refreshall/
---
## WorksheetCollection.RefreshAll method

Aggiorna tutte le tabelle pivot e i grafici con l'origine pivot.

```csharp
[Obsolete("Use Workbook.RefreshAll() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void RefreshAll()
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo Workbook.RefreshAll(). Questo metodo sarà rimosso 12 mesi dopo, a partire da aprile 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRefreshAllDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio e formule
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["B3"].PutValue(1.8);
            
            // Aggiungi formule che saranno aggiornate
            worksheet.Cells["C1"].PutValue("Total");
            worksheet.Cells["C2"].PutValue("=SUM(B2:B3)");
            
            // Modifica alcuni valori
            worksheet.Cells["B2"].PutValue(3.0);
            worksheet.Cells["B3"].PutValue(2.0);
            
            // Aggiorna tutte le formule in tutti i fogli di lavoro
            workbook.Worksheets.RefreshAll();
            
            // Genera il totale aggiornato
            Console.WriteLine("Refreshed total: " + worksheet.Cells["C2"].StringValue);
        }
    }
}
```

### Vedi anche

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


