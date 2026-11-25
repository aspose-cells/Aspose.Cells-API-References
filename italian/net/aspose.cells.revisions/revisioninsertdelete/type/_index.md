---
title: "RevisionInsertDelete.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionInsertDelete. Rappresenta il tipo di revisione"
type: docs
url: /it/net/aspose.cells.revisions/revisioninsertdelete/type/
---
## RevisionInsertDelete.Type property

Rappresenta il tipo di revisione.

```csharp
public override RevisionType Type { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertDeletePropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook e abilita il tracciamento delle revisioni
            Workbook workbook = new Workbook();
            workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 30; // Enable revision tracking by setting days

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Inserisci una riga per generare un record di revisione
            worksheet.Cells.InsertRows(0, 1);

            // Ottieni la collezione di revisioni (RevisionLogCollection stessa è la collezione)
            RevisionLogCollection revisions = workbook.Worksheets.RevisionLogs;

            // Trova il RevisionInsertDelete nelle revisioni
            foreach (RevisionLog revisionLog in revisions)
            {
                foreach (Revision revision in revisionLog.Revisions)
                {
                    if (revision is RevisionInsertDelete)
                    {
                        RevisionInsertDelete revisionInsertDelete = (RevisionInsertDelete)revision;

                        // Visualizza il valore della proprietà Type
                        Console.WriteLine("Revision Type: " + revisionInsertDelete.Type);

                        // Dimostra l'uso della proprietà Type
                        if (revisionInsertDelete.Type == RevisionType.InsertDelete)
                        {
                            Console.WriteLine("This revision represents an insert/delete operation");
                            Console.WriteLine("Affected cell area: " + revisionInsertDelete.CellArea);
                            Console.WriteLine("Action type: " + revisionInsertDelete.ActionType);
                        }

                        break;
                    }
                }
            }

            // Salva la cartella di lavoro con le revisioni
            workbook.Save("RevisionInsertDeletePropertyTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [RevisionType](../../revisiontype/)
* class [RevisionInsertDelete](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


