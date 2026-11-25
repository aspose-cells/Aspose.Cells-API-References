---
title: "Classe HighlightChangesOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Revisions.HighlightChangesOptions class. Rappresenta le opzioni di evidenziazione delle revisioni o delle modifiche dei file Excel condivisi"
type: docs
url: /it/net/aspose.cells.revisions/highlightchangesoptions/
---
## HighlightChangesOptions class

Rappresenta le opzioni per evidenziare le revisioni o le modifiche dei file Excel condivisi.

```csharp
public class HighlightChangesOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [HighlightChangesOptions](highlightchangesoptions/)(bool, bool) | Rappresenta le opzioni per evidenziare le revisioni o le modifiche dei file Excel condivisi. |

### Esempi

```csharp
using Aspose.Cells;
using Aspose.Cells.Revisions;
using System;

namespace AsposeCellsExamples
{
    public class HighlightChangesOptionsDemo
    {
        public static void HighlightChangesExample()
        {
            // Istanzia un oggetto Workbook
            Workbook workbook = new Workbook("HighlightedChangesWorkbook_original.xlsx");

            // Ottieni i registri delle revisioni
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // Imposta il numero di giorni per conservare la cronologia
            revisionLogs.DaysPreservingHistory = 30;

            // Crea HighlightChangesOptions
            HighlightChangesOptions options = new HighlightChangesOptions(true, true);

            // Evidenzia le modifiche
            revisionLogs.HighlightChanges(options);

            // Salva la cartella di lavoro con le modifiche evidenziate
            workbook.Save("HighlightedChangesWorkbook.xlsx");
            workbook.Save("HighlightedChangesWorkbook.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


