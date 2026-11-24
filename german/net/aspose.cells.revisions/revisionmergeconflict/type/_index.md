---
title: "RevisionMergeConflict.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionMergeConflict-Eigenschaft. Gibt den Typ der Revision zurück"
type: docs
url: /de/net/aspose.cells.revisions/revisionmergeconflict/type/
---
## RevisionMergeConflict.Type property

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

    public class RevisionMergeConflictPropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aktivieren Sie die Änderungsverfolgung
            workbook.StartAccessCache(AccessCacheOptions.All);

            // Nehmen Sie Änderungen vor, um ein Merge-Konfliktszenario zu erzeugen
            worksheet.Cells["A1"].PutValue("Original Value");
            workbook.Save("TempMergeConflict.xlsx");

            // Simulieren Sie einen Merge-Konflikt, indem Sie die Datei öffnen und widersprüchliche Änderungen vornehmen
            Workbook otherUserWorkbook = new Workbook("TempMergeConflict.xlsx");
            otherUserWorkbook.Worksheets[0].Cells["A1"].PutValue("Conflicting Change");
            otherUserWorkbook.Save("TempMergeConflict_OtherUser.xlsx");

            // Konfliktierende Änderungen zusammenführen
            workbook.Combine(otherUserWorkbook);

            // Überprüfen, ob Revisionen vorhanden sind
            if (workbook.HasRevisions)
            {
                // Finde die Merge-Konflikt-Revision
                RevisionMergeConflict mergeConflictRevision = null;
                // Hinweis: In der tatsächlichen Implementierung benötigen Sie eine andere Möglichkeit, um auf Revisionen zuzugreifen
                // da die Revisions-Eigenschaft in der bereitgestellten API-Definition nicht verfügbar ist

                if (mergeConflictRevision != null)
                {
                    // Zeige die Type-Eigenschaft der Merge-Konflikt-Revision an
                    Console.WriteLine("Merge Conflict Revision Type: " + mergeConflictRevision.Type);

                    // Demonstriere, wie diese Informationen verwendet werden können
                    if (mergeConflictRevision.Type == RevisionType.MergeConflict)
                    {
                        Console.WriteLine("This revision represents a merge conflict.");
                        Console.WriteLine("Worksheet affected: " + mergeConflictRevision.Worksheet.Name);
                    }
                }
            }

            // Speichern Sie die Arbeitsmappe mit Revisionen
            workbook.Save("RevisionMergeConflictTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [RevisionType](../../revisiontype/)
* class [RevisionMergeConflict](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


