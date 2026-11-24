---
title: "Aufzählung RevisionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Revisions.RevisionType Aufzählung. Stellt den Revisionstyp dar."
type: docs
url: /de/net/aspose.cells.revisions/revisiontype/
---
## RevisionType enumeration

Stellt den Revisionstyp dar.

```csharp
public enum RevisionType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| CustomView | `0` | Benutzerdefinierte Ansicht. |
| DefinedName | `1` | Definierter Name. |
| ChangeCells | `2` | Zellenänderung. |
| AutoFormat | `3` | Autoformat. |
| MergeConflict | `4` | Merge-Konflikt. |
| Comment | `5` | Kommentar. |
| Format | `6` | Format. |
| InsertSheet | `7` | Arbeitsblatt einfügen. |
| MoveCells | `8` | Zellen verschieben. |
| Undo | `9` | Rückgängig. |
| QueryTable | `10` | Abfrage‑Tabelle. |
| InsertDelete | `11` | Einfügen oder Löschen. |
| RenameSheet | `12` | Arbeitsblatt umbenennen. |
| Unknown | `13` | Unbekannt. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionTypeDemo
    {
        public static void Run()
        {
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Demonstriere die Verwendung verschiedener RevisionType‑Aufzählungswerte
                RevisionType customViewType = RevisionType.CustomView;
                RevisionType changeCellsType = RevisionType.ChangeCells;
                RevisionType insertSheetType = RevisionType.InsertSheet;

                // Zeige Aufzählungswerte und ihre zugrunde liegenden Ganzzahlwerte an
                Console.WriteLine("CustomView type: " + customViewType + " (Value: " + (int)customViewType + ")");
                Console.WriteLine("ChangeCells type: " + changeCellsType + " (Value: " + (int)changeCellsType + ")");
                Console.WriteLine("InsertSheet type: " + insertSheetType + " (Value: " + (int)insertSheetType + ")");

                // Demonstriere das Prüfen von Revisionstypen
                if (workbook.HasRevisions)
                {
                    Console.WriteLine("Workbook contains revisions");
                }
                else
                {
                    Console.WriteLine("Workbook has no revisions");
                }

                // Speichere die Arbeitsmappe
                workbook.Save("RevisionTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionType: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


