---
title: "RevisionCellChange.NewStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionCellChange. Ottiene il nuovo stile della cella"
type: docs
url: /it/net/aspose.cells.revisions/revisioncellchange/newstyle/
---
## RevisionCellChange.NewStyle property

Ottiene lo stile nuovo della cella.

```csharp
public Style NewStyle { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyNewStyleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con tracciamento delle revisioni
            Workbook workbook = new Workbook();
            // Nessun metodo StartTrackingRevisions diretto disponibile - le revisioni sono tracciate automaticamente
            Worksheet worksheet = workbook.Worksheets[0];

            // Modifica una cella per generare una revisione
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Original Value");
            Style originalStyle = workbook.CreateStyle();
            originalStyle.Font.Name = "Arial";
            originalStyle.Font.Size = 10;
            cell.SetStyle(originalStyle);

            // Cambia la cella per creare una revisione
            cell.PutValue("New Value");
            Style newStyle = workbook.CreateStyle();
            newStyle.Font.Name = "Times New Roman";
            newStyle.Font.Size = 12;
            newStyle.Font.IsBold = true;
            cell.SetStyle(newStyle);

            // Nessun metodo StopTrackingRevisions diretto disponibile

            // Accedi al registro delle revisioni tramite RevisionLogs invece di Revisions
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog log in revisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision is RevisionCellChange cellChange)
                    {
                        // Visualizza le informazioni sulla revisione della modifica della cella
                        Console.WriteLine("Cell Name: " + cellChange.CellName);
                        Console.WriteLine("Old Value: " + cellChange.OldValue);
                        Console.WriteLine("New Value: " + cellChange.NewValue);

                        // Accedi alla proprietà NewStyle
                        Style revisionNewStyle = cellChange.NewStyle;
                        Console.WriteLine("\nNew Style Properties:");
                        Console.WriteLine("Font Name: " + revisionNewStyle.Font.Name);
                        Console.WriteLine("Font Size: " + revisionNewStyle.Font.Size);
                        Console.WriteLine("Is Bold: " + revisionNewStyle.Font.IsBold);
                    }
                }
            }

            // Salva la cartella di lavoro con le revisioni
            workbook.Save("RevisionCellChangePropertyNewStyleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Style](../../../aspose.cells/style/)
* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


