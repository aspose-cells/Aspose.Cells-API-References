---
title: "RevisionInsertDelete.ActionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionInsertDelete. Restituisce il tipo di azione di questa revisione"
type: docs
url: /it/net/aspose.cells.revisions/revisioninsertdelete/actiontype/
---
## RevisionInsertDelete.ActionType property

Ottiene il tipo di azione di questa revisione.

```csharp
public RevisionActionType ActionType { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertDeletePropertyActionTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook e abilita il tracciamento delle revisioni
            Workbook workbook = new Workbook();
            workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 30;

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Esegui operazioni per generare revisioni di inserimento/cancellazione
            worksheet.Cells.InsertRows(0, 1);
            worksheet.Cells.DeleteColumn(0);

            try
            {
                // Ottieni i registri delle revisioni
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

                // Itera attraverso tutti i log di revisione per trovare revisioni di inserimento/cancellazione
                foreach (RevisionLog revisionLog in revisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionInsertDelete)
                        {
                            RevisionInsertDelete revisionInsertDelete = (RevisionInsertDelete)revision;

                            // Visualizza il valore della proprietà ActionType
                            Console.WriteLine("ActionType: " + revisionInsertDelete.ActionType);

                            // Dimostrare diversi tipi di azione
                            switch (revisionInsertDelete.ActionType)
                            {
                                case RevisionActionType.InsertRow:
                                    Console.WriteLine("This was a row insertion operation");
                                    break;
                                case RevisionActionType.DeleteColumn:
                                    Console.WriteLine("This was a column deletion operation");
                                    break;
                                case RevisionActionType.Add:
                                    Console.WriteLine("This was an add operation");
                                    break;
                                default:
                                    Console.WriteLine("This was another type of insert/delete operation");
                                    break;
                            }

                            // Mostra le informazioni correlate
                            Console.WriteLine("Affected cell area: " + revisionInsertDelete.CellArea);
                            Console.WriteLine("Revision type: " + revisionInsertDelete.Type);
                        }
                    }
                }

                // Salva la cartella di lavoro con le revisioni
                workbook.Save("ActionTypeDemo.xlsx");
                Console.WriteLine("Workbook saved with revision history.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [RevisionActionType](../../revisionactiontype/)
* class [RevisionInsertDelete](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


