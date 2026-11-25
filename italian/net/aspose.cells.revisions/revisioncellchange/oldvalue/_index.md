---
title: "RevisionCellChange.OldValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionCellChange. Restituisce il valore precedente della cella"
type: docs
url: /it/net/aspose.cells.revisions/revisioncellchange/oldvalue/
---
## RevisionCellChange.OldValue property

Ottiene il valore vecchio della cella.

```csharp
public object OldValue { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyOldValueDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati iniziali per creare una revisione
            worksheet.Cells["A1"].PutValue("Original Value");

            // Modifica la cella per creare una revisione
            worksheet.Cells["A1"].PutValue("Modified Value");

            try
            {
                // Accedi ai registri delle revisioni
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
                foreach (RevisionLog log in revisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision is RevisionCellChange cellChange)
                        {
                            // Visualizza il valore della proprietà OldValue
                            Console.WriteLine("Cell Name: " + cellChange.CellName);
                            Console.WriteLine("Old Value: " + cellChange.OldValue);
                            Console.WriteLine("New Value: " + cellChange.NewValue);

                            // Dimostra l'uso della proprietà OldValue
                            if (cellChange.OldValue != null)
                            {
                                Console.WriteLine("\nThe cell was previously set to: " + cellChange.OldValue);
                            }
                        }
                    }
                }

                // Salva la cartella di lavoro
                workbook.Save("RevisionCellChangePropertyOldValueDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
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

* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


