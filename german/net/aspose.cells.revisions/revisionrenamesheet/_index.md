---
title: "Klasse RevisionRenameSheet"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Revisions.RevisionRenameSheet Klasse. Stellt eine Revision der Umbenennung eines Arbeitsblatts dar"
type: docs
url: /de/net/aspose.cells.revisions/revisionrenamesheet/
---
## RevisionRenameSheet class

Stellt eine Revision der Umbenennung eines Arbeitsblatts dar.

```csharp
public class RevisionRenameSheet : Revision
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Ermittelt die Nummer dieser Revision.(Vererbt von [`Revision`](../revision/).) |
| [NewName](../../aspose.cells.revisions/revisionrenamesheet/newname/) { get; } | Ermittelt den neuen Namen des Arbeitsblatts. |
| [OldName](../../aspose.cells.revisions/revisionrenamesheet/oldname/) { get; } | Ermittelt den alten Namen des Arbeitsblatts. |
| override [Type](../../aspose.cells.revisions/revisionrenamesheet/type/) { get; } | Stellt den Typ der Revision dar. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Ermittelt das Arbeitsblatt.(Vererbt von [`Revision`](../revision/).) |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionRenameSheetDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Ursprünglichen Namen speichern und das Arbeitsblatt umbenennen
                string originalName = worksheet.Name;
                worksheet.Name = "RenamedSheet";

                // In einen Speicher‑Stream speichern, um Revisionen zu erzeugen
                System.IO.MemoryStream ms = new System.IO.MemoryStream();
                workbook.Save(ms, SaveFormat.Xlsx);

                // Öffnen Sie die Arbeitsmappe erneut, um auf Revisionsprotokolle zuzugreifen
                workbook = new Workbook(ms);

                // Prüfen Sie die Revisionsprotokolle für die Umbenennungsoperation
                foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision rv in log.Revisions)
                    {
                        if (rv.Type == RevisionType.RenameSheet)
                        {
                            RevisionRenameSheet renameSheet = (RevisionRenameSheet)rv;
                            Console.WriteLine("Revision Type: " + renameSheet.Type);
                            Console.WriteLine("Old Sheet Name: " + renameSheet.OldName);
                            Console.WriteLine("New Sheet Name: " + renameSheet.NewName);
                        }
                    }
                }

                // Speichere die Arbeitsmappe
                workbook.Save("RevisionRenameSheetDemo.xlsx");
                Console.WriteLine("RevisionRenameSheet demo completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in RevisionRenameSheet demo: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


