---
title: "RevisionCellChange.Column"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionCellChange. Restituisce l'indice di colonna della cella"
type: docs
url: /it/net/aspose.cells.revisions/revisioncellchange/column/
---
## RevisionCellChange.Column property

Restituisce l'indice della colonna della cella.

```csharp
public int Column { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyColumnDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con tracciamento delle revisioni
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Modifica la cella B2 per generare una revisione
            Cell cell = worksheet.Cells["B2"];
            cell.PutValue("Initial Value");

            // Cambia la cella per creare una revisione
            cell.PutValue("Modified Value");

            // Accedi ai registri delle revisioni
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog log in revisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision is RevisionCellChange cellChange)
                    {
                        // Visualizza le informazioni della colonna dalla revisione
                        Console.WriteLine("Cell Name: " + cellChange.CellName);
                        Console.WriteLine("Column Index: " + cellChange.Column);
                        Console.WriteLine("Row Index: " + cellChange.Row);

                        // Dimostra l'uso della proprietà Column
                        if (cellChange.Column == 1) // Column B is index 1
                        {
                            Console.WriteLine("\nThis revision affects column B");
                            Console.WriteLine("Old Value: " + cellChange.OldValue);
                            Console.WriteLine("New Value: " + cellChange.NewValue);
                        }
                    }
                }
            }

            // Salva la cartella di lavoro con le revisioni
            workbook.Save("RevisionCellChangePropertyColumnDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


