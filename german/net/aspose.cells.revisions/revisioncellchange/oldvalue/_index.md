---
title: "RevisionCellChange.OldValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionCellChange-Eigenschaft. Gibt den alten Wert der Zelle zurück"
type: docs
url: /de/net/aspose.cells.revisions/revisioncellchange/oldvalue/
---
## RevisionCellChange.OldValue property

Ruft den alten Wert der Zelle ab.

```csharp
public object OldValue { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Anfangsdaten hinzufügen, um eine Revision zu erstellen
            worksheet.Cells["A1"].PutValue("Original Value");

            // Zelle ändern, um eine Revision zu erstellen
            worksheet.Cells["A1"].PutValue("Modified Value");

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
                            // Zeige den Wert der OldValue-Eigenschaft an
                            Console.WriteLine("Cell Name: " + cellChange.CellName);
                            Console.WriteLine("Old Value: " + cellChange.OldValue);
                            Console.WriteLine("New Value: " + cellChange.NewValue);

                            // Demonstriere die Verwendung der OldValue-Eigenschaft
                            if (cellChange.OldValue != null)
                            {
                                Console.WriteLine("\nThe cell was previously set to: " + cellChange.OldValue);
                            }
                        }
                    }
                }

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


