---
title: "Klasse RevisionQueryTable"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Revisions.RevisionQueryTable Klasse. Stellt eine Revision einer Änderung eines Abfrage‑Tabellenfelds dar"
type: docs
url: /de/net/aspose.cells.revisions/revisionquerytable/
---
## RevisionQueryTable class

Stellt eine Revision einer Änderung eines Abfrage-Tabellenfelds dar.

```csharp
public class RevisionQueryTable : Revision
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CellArea](../../aspose.cells.revisions/revisionquerytable/cellarea/) { get; } | Ermittelt den Speicherort der betroffenen Abfrage‑Tabelle. |
| [FieldId](../../aspose.cells.revisions/revisionquerytable/fieldid/) { get; } | Ermittelt die ID des spezifischen Abfrage‑Tabellenfelds, das entfernt wurde. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Ermittelt die Nummer dieser Revision.(Vererbt von [`Revision`](../revision/).) |
| override [Type](../../aspose.cells.revisions/revisionquerytable/type/) { get; } | Stellt den Typ der Revision dar. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Ermittelt das Arbeitsblatt.(Vererbt von [`Revision`](../revision/).) |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionQueryTableDemo
    {
        public static void Run()
        {
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Füge Beispieldaten hinzu, um einen Kontext für die Abfrage‑Tabelle zu erstellen
                worksheet.Cells["A1"].Value = "Product";
                worksheet.Cells["B1"].Value = "Price";
                worksheet.Cells["A2"].Value = "Apple";
                worksheet.Cells["B2"].Value = 1.20;

                // Hinweis: RevisionQueryTable‑Instanzen werden typischerweise aus Arbeitsmappen‑Revisionen erhalten
                // Dies ist eine konzeptionelle Demonstration, da wir RevisionQueryTable nicht direkt instanziieren können

                // In einem realen Szenario würdest du Revisionen wie folgt zugreifen:
                // RevisionCollection revisions = workbook.Worksheets.Revisions;
                // foreach (Revision revision in revisions)
                // {
                //     if (revision is RevisionQueryTable queryTableRevision)
                //     {
                //         // Zugriff auf Eigenschaften
                //     }
                // }

                // Zur Demonstration zeigen wir, wie man mit den Eigenschaften von RevisionQueryTable arbeitet
                // wenn wir eine Instanz hätten
                Console.WriteLine("RevisionQueryTable properties demonstration:");
                Console.WriteLine("Type property would return: " + RevisionType.QueryTable);
                Console.WriteLine("FieldId property would return an integer ID of the affected field");
                Console.WriteLine("CellArea property would return the location of the query table");

                // Speichere die Arbeitsmappe
                workbook.Save("RevisionQueryTableDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionQueryTable: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


