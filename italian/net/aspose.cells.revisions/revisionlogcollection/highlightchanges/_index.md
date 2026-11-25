---
title: "RevisionLogCollection.HighlightChanges"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo RevisionLogCollection. Evidenzia le modifiche della cartella di lavoro condivisa"
type: docs
url: /it/net/aspose.cells.revisions/revisionlogcollection/highlightchanges/
---
## RevisionLogCollection.HighlightChanges method

Evidenzia le modifiche della cartella di lavoro condivisa.

```csharp
public void HighlightChanges(HighlightChangesOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opzioni | HighlightChangesOptions | Imposta le opzioni per filtrare quali modifiche devono essere tracciate. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionLogCollectionMethodHighlightChangesWithHighlightChangesOptionsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati di esempio e revisioni
            worksheet.Cells["A1"].PutValue("Original Value");
            worksheet.Cells["A1"].PutValue("Modified Value");
            
            // Evidenzia le modifiche con le opzioni
            HighlightChangesOptions options = new HighlightChangesOptions(true, true);
            workbook.Worksheets.RevisionLogs.HighlightChanges(options);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [HighlightChangesOptions](../../highlightchangesoptions/)
* class [RevisionLogCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


