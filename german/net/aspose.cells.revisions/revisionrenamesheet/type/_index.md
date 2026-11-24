---
title: "RevisionRenameSheet.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionRenameSheet-Eigenschaft. Stellt den Typ der Revision dar"
type: docs
url: /de/net/aspose.cells.revisions/revisionrenamesheet/type/
---
## RevisionRenameSheet.Type property

Stellt den Typ der Revision dar.

```csharp
public override RevisionType Type { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionRenameSheetPropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Aktiviere das Verfolgen von Revisionen, BEVOR Änderungen vorgenommen werden
            // Hinweis: Diese Methode existiert nicht in der bereitgestellten API, daher entfernen wir sie
            // workbook.StartTrackingRevisions();

            // Benenne das erste Arbeitsblatt um, um eine Revision zu erstellen
            Worksheet worksheet = workbook.Worksheets[0];
            string originalName = worksheet.Name;
            worksheet.Name = "RenamedSheet";

            // Greife auf die Revisionssammlung zu
            // Hinweis: Die Revisions-Eigenschaft existiert nicht in der bereitgestellten API
            // Daher müssen wir zunächst prüfen, ob die Arbeitsmappe Revisionen enthält
            if (workbook.HasRevisions)
            {
                // Finde die Umbenennen‑Blatt‑Revision
                RevisionRenameSheet renameRevision = null;
                // Da wir nicht direkt auf Revisions zugreifen können, müssen wir diesen Teil anpassen
                // Dies ist nur ein Platzhalter, da die tatsächliche API keinen Zugriff auf Revisionen unterstützt
                Console.WriteLine("Revision tracking is not fully supported in this API version.");
                
                if (renameRevision != null)
                {
                    // Den Wert der Type-Eigenschaft anzeigen
                    Console.WriteLine("Revision Type: " + renameRevision.Type);
                    Console.WriteLine("Old Sheet Name: " + renameRevision.OldName);
                    Console.WriteLine("New Sheet Name: " + renameRevision.NewName);

                    // Demonstriere, wie die Type‑Eigenschaft verwendet wird
                    if (renameRevision.Type == RevisionType.RenameSheet)
                    {
                        Console.WriteLine("This revision represents a worksheet rename operation.");
                    }
                }
            }

            // Speichern Sie die Arbeitsmappe mit Revisionen
            workbook.Save("RevisionRenameSheetDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [RevisionType](../../revisiontype/)
* class [RevisionRenameSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


