---
title: "RevisionInsertSheet.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionInsertSheet‑Eigenschaft. Gibt den Typ der Revision zurück"
type: docs
url: /de/net/aspose.cells.revisions/revisioninsertsheet/type/
---
## RevisionInsertSheet.Type property

Liest den Typ der Revision.

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

    public class RevisionInsertSheetPropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe mit Revisionsverfolgung
            Workbook workbook = new Workbook();
            
            // Aktivieren Sie die Revisionsverfolgung (simuliert, da StartTrackingRevisions nicht verfügbar ist)
            bool trackRevisions = true;

            // Fügen Sie ein neues Arbeitsblatt hinzu, um einen Revisionsdatensatz zu erstellen
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");
            
            // Simulieren Sie das Abrufen von Revisionen (da die Revisions‑Eigenschaft nicht verfügbar ist)
            if (trackRevisions && workbook.HasRevisions)
            {
                // In einem realen Szenario würden wir hier auf die Revisionen zugreifen
                // Dies setzt voraus, dass wir die Revision von irgendwo erhalten haben (z. B. workbook.Revisions)
                RevisionInsertSheet insertSheetRevision = null; // Would be assigned from actual revisions collection
                
                if (insertSheetRevision != null)
                {
                    // Zeige die Type‑Eigenschaft an
                    Console.WriteLine("Revision Type: " + insertSheetRevision.Type);

                    // Demonstriere die Verwendung der schreibgeschützten Type‑Eigenschaft
                    if (insertSheetRevision.Type == RevisionType.InsertSheet)
                    {
                        Console.WriteLine("This revision represents a sheet insertion operation");
                        
                        // Zeige zusätzliche Informationen zum eingefügten Blatt an
                        Console.WriteLine("Inserted sheet name: " + insertSheetRevision.Name);
                        Console.WriteLine("Sheet position: " + insertSheetRevision.SheetPosition);
                    }

                    // Überprüfe gegenüber anderen Revisionsarten
                    if (insertSheetRevision.Type != RevisionType.Unknown)
                    {
                        Console.WriteLine("This is a known revision type");
                    }
                }

                // Speichere die Arbeitsmappe
                workbook.Save("RevisionInsertSheetTypeDemo.xlsx");
            }
            else
            {
                Console.WriteLine("No revisions found or revision tracking not enabled");
            }
        }
    }
}
```

### Siehe auch

* enum [RevisionType](../../revisiontype/)
* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


