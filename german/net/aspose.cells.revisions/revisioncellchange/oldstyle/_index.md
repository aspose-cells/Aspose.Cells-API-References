---
title: "RevisionCellChange.OldStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionCellChange-Eigenschaft. Gibt den alten Stil der Zelle zurück"
type: docs
url: /de/net/aspose.cells.revisions/revisioncellchange/oldstyle/
---
## RevisionCellChange.OldStyle property

Ruft den alten Stil der Zelle ab.

```csharp
public Style OldStyle { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyOldStyleDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe mit Revisionsverfolgung
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Initialen Stil für Zelle A1 festlegen
            Cell cell = worksheet.Cells["A1"];
            Style initialStyle = workbook.CreateStyle();
            initialStyle.Font.Name = "Arial";
            initialStyle.Font.Size = 10;
            initialStyle.Font.Color = System.Drawing.Color.Black;
            cell.SetStyle(initialStyle);
            cell.PutValue("Initial Value");

            // Zellstil ändern, um eine Revision zu erstellen
            Style newStyle = workbook.CreateStyle();
            newStyle.Font.Name = "Times New Roman";
            newStyle.Font.Size = 12;
            newStyle.Font.Color = System.Drawing.Color.Red;
            newStyle.Font.IsBold = true;
            cell.SetStyle(newStyle);
            cell.PutValue("Modified Value");

            // Greife auf die Revisionsprotokolle zu
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog log in revisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision is RevisionCellChange cellChange && cellChange.CellName == "A1")
                    {
                        // Informationen zur Stiländerung anzeigen
                        Console.WriteLine("Cell Name: " + cellChange.CellName);
                        Console.WriteLine("Old Style Font: " + cellChange.OldStyle.Font.Name);
                        Console.WriteLine("Old Style Size: " + cellChange.OldStyle.Font.Size);
                        Console.WriteLine("Old Style Color: " + cellChange.OldStyle.Font.Color);
                        Console.WriteLine("New Style Font: " + cellChange.NewStyle.Font.Name);
                        Console.WriteLine("New Style Size: " + cellChange.NewStyle.Font.Size);
                        Console.WriteLine("New Style Color: " + cellChange.NewStyle.Font.Color);

                        // Demonstrieren Sie die Verwendung der OldStyle-Eigenschaft
                        if (cellChange.OldStyle.Font.Name == "Arial")
                        {
                            Console.WriteLine("\nThe cell originally had Arial font");
                        }
                    }
                }
            }

            // Speichern Sie die Arbeitsmappe mit Revisionen
            workbook.Save("RevisionCellChangePropertyOldStyleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../../../aspose.cells/style/)
* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


