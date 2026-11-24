---
title: "RevisionCellChange.Column"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionCellChange-Eigenschaft. Gibt den Spaltenindex der Zelle zurück"
type: docs
url: /de/net/aspose.cells.revisions/revisioncellchange/column/
---
## RevisionCellChange.Column property

Liefert den Spaltenindex der Zelle.

```csharp
public int Column { get; }
```

### Beispiele

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
            // Erstelle eine neue Arbeitsmappe mit Revisionsverfolgung
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ändere die Zelle B2, um eine Revision zu erzeugen
            Cell cell = worksheet.Cells["B2"];
            cell.PutValue("Initial Value");

            // Ändere die Zelle, um eine Revision zu erstellen
            cell.PutValue("Modified Value");

            // Greife auf die Revisionsprotokolle zu
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog log in revisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision is RevisionCellChange cellChange)
                    {
                        // Zeige Spalteninformationen aus der Revision an
                        Console.WriteLine("Cell Name: " + cellChange.CellName);
                        Console.WriteLine("Column Index: " + cellChange.Column);
                        Console.WriteLine("Row Index: " + cellChange.Row);

                        // Demonstriere die Verwendung der Column-Eigenschaft
                        if (cellChange.Column == 1) // Column B is index 1
                        {
                            Console.WriteLine("\nThis revision affects column B");
                            Console.WriteLine("Old Value: " + cellChange.OldValue);
                            Console.WriteLine("New Value: " + cellChange.NewValue);
                        }
                    }
                }
            }

            // Speichern Sie die Arbeitsmappe mit Revisionen
            workbook.Save("RevisionCellChangePropertyColumnDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


