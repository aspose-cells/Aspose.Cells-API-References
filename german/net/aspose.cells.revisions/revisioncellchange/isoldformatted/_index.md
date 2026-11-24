---
title: "RevisionCellChange.IsOldFormatted"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionCellChange-Eigenschaft. Gibt an, ob diese Zelle alt formatiert ist"
type: docs
url: /de/net/aspose.cells.revisions/revisioncellchange/isoldformatted/
---
## RevisionCellChange.IsOldFormatted property

Gibt an, ob diese Zelle bereits formatiert ist.

```csharp
public bool IsOldFormatted { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyIsOldFormattedDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
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

            try
            {
                // Greife auf die Revisionsprotokolle zu
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
                foreach (RevisionLog log in revisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision is RevisionCellChange cellChange)
                        {
                            // IsOldFormatted-Eigenschaftswert anzeigen
                            Console.WriteLine("Cell Name: " + cellChange.CellName);
                            Console.WriteLine("IsOldFormatted: " + cellChange.IsOldFormatted);

                            // Zusätzlichen Kontext zur Revision anzeigen
                            if (cellChange.IsOldFormatted)
                            {
                                Console.WriteLine("The cell had formatting before this revision.");
                                Console.WriteLine("Old Font: " + cellChange.OldStyle.Font.Name);
                                Console.WriteLine("Old Font Size: " + cellChange.OldStyle.Font.Size);
                            }
                            else
                            {
                                Console.WriteLine("The cell did not have formatting before this revision.");
                            }
                        }
                    }
                }

                // Speichern Sie die Arbeitsmappe mit Revisionen
                workbook.Save("IsOldFormattedDemo.xlsx");
                Console.WriteLine("Demo completed successfully. File saved as IsOldFormattedDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


