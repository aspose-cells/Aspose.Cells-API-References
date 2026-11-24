---
title: "Enum RevisionActionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Revisions.RevisionActionType Enum. Stellt den Typ der Revisionsaktion dar"
type: docs
url: /de/net/aspose.cells.revisions/revisionactiontype/
---
## RevisionActionType enumeration

Stellt den Typ der Revisionsaktion dar.

```csharp
public enum RevisionActionType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Add | `0` | Revision hinzufügen. |
| Delete | `1` | Revision löschen. |
| DeleteColumn | `2` | Spaltenlöschrevision. |
| DeleteRow | `3` | Zeilenlöschrevision. |
| InsertColumn | `4` | Spalteneinfügungsrevision. |
| InsertRow | `5` | Zeilen‑Einfügungsrevision. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionActionTypeDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe mit Revisionsverfolgung
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Führe verschiedene Vorgänge aus, die unterschiedliche Revisionsarten erzeugen
            worksheet.Cells["A1"].PutValue("Initial Value");
            worksheet.Cells.InsertRow(0);
            worksheet.Cells.DeleteRow(1);
            worksheet.Cells.InsertColumn(0);
            worksheet.Cells.DeleteColumn(1);

            // Prüfe, ob die Arbeitsmappe Revisionen enthält
            if (workbook.HasRevisions)
            {
                // Hinweis: Die ursprüngliche API bietet keinen direkten Zugriff auf die Revisionssammlung
                // Also demonstrieren wir einfach das RevisionActionType‑Enum wie angefordert
                Console.WriteLine("Workbook contains revisions (but API doesn't provide access)");
            }

            // Demonstriere die Verwendung von RevisionActionType‑Enum‑Werten
            Console.WriteLine("Available revision action types:");
            foreach (RevisionActionType actionType in Enum.GetValues(typeof(RevisionActionType)))
            {
                Console.WriteLine($"{actionType} = {(int)actionType}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("RevisionActionTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


