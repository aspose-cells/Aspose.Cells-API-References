---
title: "RevisionCellChange.IsNewFormatted"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionCellChange-Eigenschaft. Gibt an, ob diese Zelle neu formatiert ist"
type: docs
url: /de/net/aspose.cells.revisions/revisioncellchange/isnewformatted/
---
## RevisionCellChange.IsNewFormatted property

Gibt an, ob diese Zelle neu formatiert ist.

```csharp
public bool IsNewFormatted { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyIsNewFormattedDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe mit Revisionsverfolgung
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Initialen Zellenwert und Stil festlegen
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Initial Value");
            Style initialStyle = workbook.CreateStyle();
            initialStyle.Font.Name = "Arial";
            initialStyle.Font.Size = 10;
            cell.SetStyle(initialStyle);

            // Zellenwert und Stil ändern, um eine Revision zu erstellen
            cell.PutValue("Updated Value");
            Style newStyle = workbook.CreateStyle();
            newStyle.Font.Name = "Calibri";
            newStyle.Font.Size = 12;
            newStyle.Font.IsBold = true;
            cell.SetStyle(newStyle);

            // Greife auf die Revisionsprotokolle zu
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog log in revisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision is RevisionCellChange cellChange)
                    {
                        // Zeige Revisionsinformationen an
                        Console.WriteLine("Cell Name: " + cellChange.CellName);
                        Console.WriteLine("Old Value: " + cellChange.OldValue);
                        Console.WriteLine("New Value: " + cellChange.NewValue);

                        // Demonstriere die IsNewFormatted-Eigenschaft
                        Console.WriteLine("\nFormatting Information:");
                        Console.WriteLine("IsOldFormatted: " + cellChange.IsOldFormatted);
                        Console.WriteLine("IsNewFormatted: " + cellChange.IsNewFormatted);

                        if (cellChange.IsNewFormatted)
                        {
                            Console.WriteLine("The cell has new formatting applied in this revision.");
                            Console.WriteLine("New Font: " + cellChange.NewStyle.Font.Name);
                            Console.WriteLine("New Font Size: " + cellChange.NewStyle.Font.Size);
                            Console.WriteLine("Is Bold: " + cellChange.NewStyle.Font.IsBold);
                        }
                    }
                }
            }

            // Speichern Sie die Arbeitsmappe mit Revisionen
            workbook.Save("RevisionCellChangePropertyIsNewFormattedDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


