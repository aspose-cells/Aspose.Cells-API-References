---
title: "RevisionCellChange.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionCellChange. Rappresenta il tipo di revisione"
type: docs
url: /it/net/aspose.cells.revisions/revisioncellchange/type/
---
## RevisionCellChange.Type property

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

    public class RevisionCellChangePropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con tracciamento delle revisioni
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Abilita il tracciamento delle modifiche modificando una cella - le revisioni vengono tracciate automaticamente
            // quando le modifiche vengono apportate dopo la creazione della cartella di lavoro
            Cell cell = worksheet.Cells["A1"];
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
                        // Visualizza le informazioni del tipo dalla revisione
                        Console.WriteLine("Cell Name: " + cellChange.CellName);
                        Console.WriteLine("Revision Type: " + cellChange.Type);

                        // Dimostra l'uso della proprietà Type
                        if (cellChange.Type == RevisionType.ChangeCells)
                        {
                            Console.WriteLine("\nThis is a cell change revision");
                            Console.WriteLine("Old Value: " + cellChange.OldValue);
                            Console.WriteLine("New Value: " + cellChange.NewValue);
                        }

                        // Verifica altri possibili tipi di revisione
                        switch (cellChange.Type)
                        {
                            case RevisionType.ChangeCells:
                                Console.WriteLine("Handling cell value change revision");
                                break;
                            case RevisionType.Format:
                                Console.WriteLine("Handling format change revision");
                                break;
                            default:
                                Console.WriteLine("Handling other type of revision");
                                break;
                        }
                    }
                }
            }

            // Salva la cartella di lavoro con le revisioni
            workbook.Save("RevisionCellChangePropertyTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [RevisionType](../../revisiontype/)
* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


