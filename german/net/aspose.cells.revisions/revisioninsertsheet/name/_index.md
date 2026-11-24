---
title: "RevisionInsertSheet.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionInsertSheet‑Eigenschaft. Gibt den Namen des Arbeitsblatts zurück"
type: docs
url: /de/net/aspose.cells.revisions/revisioninsertsheet/name/
---
## RevisionInsertSheet.Name property

Liest den Namen des Arbeitsblatts.

```csharp
public string Name { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertSheetPropertyNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Fügen Sie ein neues Arbeitsblatt hinzu, um möglicherweise einen Revisionsdatensatz zu erzeugen
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");

            try
            {
                // Simulieren Sie den Zugriff auf ein RevisionInsertSheet aus den Revisionen
                // Hinweis: In einem echten Szenario würde dies aus workbook.Revisions stammen
                // Zur Demonstration erstellen wir ein Mock‑Szenario
                RevisionInsertSheet insertSheetRevision = null;

                // Im tatsächlichen Gebrauch würden Sie dies aus der Revisionssammlung erhalten
                // Beispiel: insertSheetRevision = (RevisionInsertSheet)workbook.Revisions[0];

                // Da wir RevisionInsertSheet nicht direkt erstellen können, demonstrieren wir dies
                // was Sie tun würden, wenn Sie Zugriff darauf hätten
                if (insertSheetRevision != null)
                {
                    // Zeigen Sie den Wert der Name‑Eigenschaft an (schreibgeschützt)
                    Console.WriteLine("Inserted sheet name: " + insertSheetRevision.Name);

                    // Demonstrieren Sie die Verwendung der Name‑Eigenschaft in einer Bedingungsprüfung
                    if (!string.IsNullOrEmpty(insertSheetRevision.Name))
                    {
                        Console.WriteLine("The sheet has a valid name: " + insertSheetRevision.Name);
                    }
                }
                else
                {
                    Console.WriteLine("No RevisionInsertSheet found in revisions");
                }

                // Speichere die Arbeitsmappe
                workbook.Save("RevisionInsertSheetNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
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

* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


