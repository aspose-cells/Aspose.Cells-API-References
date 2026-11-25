---
title: "RevisionCellChange.CellName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionCellChange. Restituisce il nome della cella"
type: docs
url: /it/net/aspose.cells.revisions/revisioncellchange/cellname/
---
## RevisionCellChange.CellName property

Ottiene il nome della cella.

```csharp
public string CellName { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyCellNameDemo
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
                            // Visualizza il valore della proprietà CellName
                            Console.WriteLine("Cell Name: " + cellChange.CellName);
                            Console.WriteLine("Row Index: " + cellChange.Row);
                            Console.WriteLine("Column Index: " + cellChange.Column);

                            // Dimostra l'uso della proprietà CellName
                            if (cellChange.CellName == "A1")
                            {
                                Console.WriteLine("\nThe revision is for cell A1");
                                Console.WriteLine("Old Value: " + cellChange.OldValue);
                                Console.WriteLine("New Value: " + cellChange.NewValue);
                            }
                        }
                    }
                }

                // Salva la cartella di lavoro
                workbook.Save("RevisionCellChangePropertyCellNameDemo.xlsx");
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


