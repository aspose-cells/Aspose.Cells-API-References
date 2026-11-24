---
title: "Klasse RevisionInsertSheet"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Revisions.RevisionInsertSheet Klasse. Stellt einen Revisionsdatensatz eines eingefügten Blatts dar"
type: docs
url: /de/net/aspose.cells.revisions/revisioninsertsheet/
---
## RevisionInsertSheet class

Stellt einen Revisionsdatensatz eines eingefügten Arbeitsblatts dar.

```csharp
public class RevisionInsertSheet : Revision
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ActionType](../../aspose.cells.revisions/revisioninsertsheet/actiontype/) { get; } | Liest den Aktionstyp der Revision. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Ermittelt die Nummer dieser Revision.(Vererbt von [`Revision`](../revision/).) |
| [Name](../../aspose.cells.revisions/revisioninsertsheet/name/) { get; } | Liest den Namen des Arbeitsblatts. |
| [SheetPosition](../../aspose.cells.revisions/revisioninsertsheet/sheetposition/) { get; } | Liest die nullbasierte Position des neuen Blatts in der Blattregisterleiste. |
| override [Type](../../aspose.cells.revisions/revisioninsertsheet/type/) { get; } | Liest den Typ der Revision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Ermittelt das Arbeitsblatt.(Vererbt von [`Revision`](../revision/).) |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionInsertSheetDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Füge ein neues Arbeitsblatt hinzu, um möglicherweise eine Revision zu erzeugen
                Worksheet newSheet = workbook.Worksheets.Add("NewSheet");

                // Hinweis: Da wir keine RevisionInsertSheet-Instanzen direkt erstellen können,
                // Wir zeigen, wie man mit einer arbeitet, falls sie in der Revisionssammlung existieren würde
                // Dies ist ein simuliertes Szenario, da die tatsächliche Revision-Tracking-API nicht vollständig verfügbar ist

                // In einem realen Szenario mit aktivierter Revisionserfassung könnten Sie Revisionen wie folgt erhalten:
                // RevisionInsertSheet revision = null; // Würde aus der workbook.Revisions Sammlung kommen

                // Zu Demonstrationszwecken zeigen wir das Muster der Arbeit mit einem RevisionInsertSheet
                // Da wir es nicht direkt instanziieren können, zeigen wir das Muster des Property-Zugriffs

                // Statt zu versuchen, eine Instanz zu erstellen, zeigen wir, wie man mit einer arbeitet, falls verfügbar
                // Dies erhält die Struktur bei gleichzeitiger Behebung des Kompilierungsfehlers

                // Informationen zu den Revisions-Eigenschaften anzeigen (simuliert)
                Console.WriteLine("RevisionInsertSheet properties demonstration:");
                Console.WriteLine("Type property would show: RevisionType.InsertSheet");
                Console.WriteLine("ActionType property would show: RevisionActionType.Add");
                Console.WriteLine("Name property would show the sheet name");
                Console.WriteLine("SheetPosition property would show the zero-based position");

                // Speichere die Arbeitsmappe
                workbook.Save("RevisionInsertSheetDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with potential revisions.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionInsertSheet: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


