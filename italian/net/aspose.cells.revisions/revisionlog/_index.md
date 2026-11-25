---
title: "Classe RevisionLog"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Revisions.RevisionLog. Rappresenta il log delle revisioni"
type: docs
url: /it/net/aspose.cells.revisions/revisionlog/
---
## RevisionLog class

Rappresenta il registro delle revisioni.

```csharp
public class RevisionLog
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [MetadataTable](../../aspose.cells.revisions/revisionlog/metadatatable/) { get; } | Ottiene la tabella che contiene i metadati su un elenco di modifiche specifiche avvenute per questa cartella di lavoro. |
| [Revisions](../../aspose.cells.revisions/revisionlog/revisions/) { get; } | Ottiene tutte le revisioni in questo log. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionLogDemo
    {
        public static void RevisionLogExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook("HighlightedChangesWorkbook_original.xlsx");

            // Accedi ai log delle revisioni della cartella di lavoro
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // Verifica se ci sono log di revisione
            if (revisionLogs.Count > 0)
            {
                // Accedi al primo log delle revisioni
                RevisionLog revisionLog = revisionLogs[0];

                // Accedi alla tabella dei metadati del log delle revisioni
                RevisionHeader metadataTable = revisionLog.MetadataTable;

                // Accedi alle revisioni nel log delle revisioni
                RevisionCollection revisions = revisionLog.Revisions;

                // Visualizza alcune informazioni sulle revisioni
                Console.WriteLine("Number of revisions: " + revisions.Count);
                Console.WriteLine("Metadata Table: " + metadataTable.ToString());
            }
            else
            {
                Console.WriteLine("No revision logs found.");
            }

            // Salva la cartella di lavoro
            workbook.Save("RevisionLogExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


