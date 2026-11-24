---
title: "RevisionQueryTable.FieldId"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionQueryTable-Eigenschaft. Gibt die ID des spezifischen Abfrage-Tabellenfeldes zurück, das entfernt wurde"
type: docs
url: /de/net/aspose.cells.revisions/revisionquerytable/fieldid/
---
## RevisionQueryTable.FieldId property

Ermittelt die ID des spezifischen Abfrage‑Tabellenfelds, das entfernt wurde.

```csharp
public int FieldId { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionQueryTablePropertyFieldIdDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Beispieldaten zum Arbeitsblatt hinzu
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 1.20;

            try
            {
                // Erstelle eine Abfrage-Tabelle (dies ist ein vereinfachtes Beispiel)
                // Hinweis: In einem realen Szenario müssten Sie zuerst eine Abfrage-Tabelle erstellen
                // Zu Demonstrationszwecken simulieren wir den Zugriff auf eine RevisionQueryTable

                // Da wir in diesem vereinfachten Beispiel keine RevisionQueryTable direkt erstellen können,
                // zeigen wir, wie man auf die FieldId-Eigenschaft zugreifen würde, falls wir eine hätten
                // Dies zeigt das Muster zum Lesen der schreibgeschützten Eigenschaft

                // Simuliere das Abrufen einer RevisionQueryTable aus Revisionen (konzeptionell)
                // In der Praxis würden Sie dies von workbook.Revisions oder Ähnlichem erhalten
                RevisionQueryTable revisionQueryTable = null;

                // Prüfen Sie, ob wir eine RevisionQueryTable haben (dies ist nur zur Demonstration)
                if (revisionQueryTable != null)
                {
                    // Zeige den Wert der FieldId-Eigenschaft an
                    Console.WriteLine("FieldId value: " + revisionQueryTable.FieldId);

                    // Zeige weitere Eigenschaften für den Kontext an
                    Console.WriteLine("Revision Type: " + revisionQueryTable.Type);
                    Console.WriteLine("Cell Area: " + revisionQueryTable.CellArea);
                }
                else
                {
                    Console.WriteLine("No RevisionQueryTable available in this example.");
                    Console.WriteLine("In a real scenario, you would access this from workbook revisions.");
                }

                // Speichere die Arbeitsmappe
                workbook.Save("FieldIdDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [RevisionQueryTable](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


