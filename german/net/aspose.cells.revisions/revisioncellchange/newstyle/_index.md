---
title: "RevisionCellChange.NewStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionCellChange-Eigenschaft. Gibt den neuen Stil der Zelle zurück"
type: docs
url: /de/net/aspose.cells.revisions/revisioncellchange/newstyle/
---
## RevisionCellChange.NewStyle property

Ruft den neuen Stil der Zelle ab.

```csharp
public Style NewStyle { get; }
```

### Beispiele

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
            // Erstelle eine neue Arbeitsmappe mit Revisionsverfolgung
            Workbook workbook = new Workbook();
            // Keine direkte StartTrackingRevisions‑Methode verfügbar – Revisionen werden automatisch verfolgt
            Worksheet worksheet = workbook.Worksheets[0];

            // Modifiziere eine Zelle, um eine Revision zu erzeugen
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Original Value");
            Style originalStyle = workbook.CreateStyle();
            originalStyle.Font.Name = "Arial";
            originalStyle.Font.Size = 10;
            cell.SetStyle(originalStyle);

            // Ändere die Zelle, um eine Revision zu erstellen
            cell.PutValue("New Value");
            Style newStyle = workbook.CreateStyle();
            newStyle.Font.Name = "Times New Roman";
            newStyle.Font.Size = 12;
            newStyle.Font.IsBold = true;
            cell.SetStyle(newStyle);

            // Keine direkte StopTrackingRevisions‑Methode verfügbar

            // Greife über RevisionLogs statt über Revisions auf das Revisionsprotokoll zu
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog log in revisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision is RevisionCellChange cellChange)
                    {
                        // Zeige Informationen zur Zelländerungs‑Revision an
                        Console.WriteLine("Cell Name: " + cellChange.CellName);
                        Console.WriteLine("Old Value: " + cellChange.OldValue);
                        Console.WriteLine("New Value: " + cellChange.NewValue);

                        // Greife auf die NewStyle‑Eigenschaft zu
                        Style revisionNewStyle = cellChange.NewStyle;
                        Console.WriteLine("\nNew Style Properties:");
                        Console.WriteLine("Font Name: " + revisionNewStyle.Font.Name);
                        Console.WriteLine("Font Size: " + revisionNewStyle.Font.Size);
                        Console.WriteLine("Is Bold: " + revisionNewStyle.Font.IsBold);
                    }
                }
            }

            // Speichern Sie die Arbeitsmappe mit Revisionen
            workbook.Save("RevisionCellChangePropertyNewStyleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../../../aspose.cells/style/)
* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


