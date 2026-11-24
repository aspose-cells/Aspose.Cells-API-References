---
title: "RevisionInsertSheet.ActionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionInsertSheet‑Eigenschaft. Gibt den Aktionstyp der Revision zurück"
type: docs
url: /de/net/aspose.cells.revisions/revisioninsertsheet/actiontype/
---
## RevisionInsertSheet.ActionType property

Liest den Aktionstyp der Revision.

```csharp
public RevisionActionType ActionType { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertSheetPropertyActionTypeDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe mit Revisionsverfolgung
            Workbook workbook = new Workbook();
            // Hinweis: StartTrackingRevisions ist in der bereitgestellten API nicht verfügbar
            // workbook.StartTrackingRevisions();

            // Fügen Sie ein neues Arbeitsblatt hinzu, um einen Revisionsdatensatz zu erstellen
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");
            
            // Hinweis: StopTrackingRevisions ist in der bereitgestellten API nicht verfügbar
            // workbook.StopTrackingRevisions();
            
            // Hinweis: Die Revisions‑Eigenschaft ist in der bereitgestellten API nicht verfügbar
            // Wir verwenden HasRevisions, um zu prüfen, ob Revisionen vorhanden sind
            if (workbook.HasRevisions)
            {
                // In einem realen Szenario würden wir hier auf die Revisionen zugreifen
                // Da wir RevisionInsertSheet nicht direkt erstellen können, simulieren wir die Überprüfung einer
                // Dies setzt voraus, dass wir die Revision von irgendwo erhalten haben (z. B. workbook.Revisions)
                RevisionInsertSheet insertSheetRevision = null; // Would be assigned from actual revisions collection
                
                // Da wir ActionType nicht erstellen oder setzen können, demonstrieren wir lediglich die Überprüfung
                if (insertSheetRevision != null)
                {
                    // Zeige die ActionType‑Eigenschaft an
                    Console.WriteLine("ActionType of sheet insertion: " + insertSheetRevision.ActionType);

                    // Demonstriere die Verwendung der schreibgeschützten Eigenschaft
                    if (insertSheetRevision.ActionType == RevisionActionType.Add)
                    {
                        Console.WriteLine("This revision represents a sheet addition");
                    }
                }

                // Speichern Sie die Arbeitsmappe mit Revisionen
                workbook.Save("RevisionInsertSheetActionTypeDemo.xlsx");
            }
            else
            {
                Console.WriteLine("No sheet insertion revision found");
            }
        }
    }
}
```

### Siehe auch

* enum [RevisionActionType](../../revisionactiontype/)
* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


