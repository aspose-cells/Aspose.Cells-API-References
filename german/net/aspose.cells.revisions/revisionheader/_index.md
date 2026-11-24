---
title: "Klasse RevisionHeader"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Revisions.RevisionHeader Klasse. Stellt eine Liste spezifischer Änderungen dar, die für diese Arbeitsmappe vorgenommen wurden."
type: docs
url: /de/net/aspose.cells.revisions/revisionheader/
---
## RevisionHeader class

Stellt eine Liste spezifischer Änderungen dar, die für diese Arbeitsmappe vorgenommen wurden.

```csharp
public class RevisionHeader
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [RevisionHeader](revisionheader/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [SavedTime](../../aspose.cells.revisions/revisionheader/savedtime/) { get; set; } | Liest und setzt das Datum und die Uhrzeit, wann dieser Satz von Revisionen gespeichert wurde. |
| [UserName](../../aspose.cells.revisions/revisionheader/username/) { get; set; } | Liest und setzt den Namen des Benutzers, der die Revision vornimmt. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionHeaderDemo
    {
        public static void Run()
        {
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Erstelle eine Instanz der RevisionHeader-Klasse
                RevisionHeader revisionHeader = new RevisionHeader();

                // Setze wesentliche Eigenschaften
                revisionHeader.SavedTime = DateTime.Now;
                revisionHeader.UserName = "TestUser";

                // Demonstriere grundlegende Funktionalität
                Console.WriteLine($"Revision saved by: {revisionHeader.UserName}");
                Console.WriteLine($"Revision saved at: {revisionHeader.SavedTime}");

                // Speichere die Arbeitsmappe
                workbook.Save("RevisionHeaderDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with revision header information.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionHeader: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


