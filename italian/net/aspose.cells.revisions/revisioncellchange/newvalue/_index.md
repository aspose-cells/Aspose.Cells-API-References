---
title: "RevisionCellChange.NewValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionCellChange. Ottiene il nuovo valore della cella"
type: docs
url: /it/net/aspose.cells.revisions/revisioncellchange/newvalue/
---
## RevisionCellChange.NewValue property

Ottiene il nuovo valore della cella.

```csharp
public object NewValue { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyNewValueDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi i dati iniziali alla cella A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Original Value");

            // Modifica la cella per creare una revisione
            cell.PutValue("Modified Value");

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
                            // Visualizza la proprietà NewValue
                            Console.WriteLine("Cell Name: " + cellChange.CellName);
                            Console.WriteLine("Old Value: " + cellChange.OldValue);
                            Console.WriteLine("New Value: " + cellChange.NewValue);

                            // Dimostra l'uso della proprietà NewValue
                            if (cellChange.NewValue != null)
                            {
                                Console.WriteLine("\nThe new value is: " + cellChange.NewValue.ToString());
                            }
                        }
                    }
                }

                // Salva la cartella di lavoro con le revisioni
                workbook.Save("RevisionCellChangePropertyNewValueDemo.xlsx");
                Console.WriteLine("\nWorkbook saved with revisions.");
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


