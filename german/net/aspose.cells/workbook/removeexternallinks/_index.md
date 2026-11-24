---
title: "Workbook.RemoveExternalLinks"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Entfernt alle externen Links in der Arbeitsmappe"
type: docs
url: /de/net/aspose.cells/workbook/removeexternallinks/
---
## Workbook.RemoveExternalLinks method

Entfernt alle externen Links in der Arbeitsmappe.

```csharp
[Obsolete("Use ExternalLinkCollection.Clear() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void RemoveExternalLinks()
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode ExternalLinkCollection.Clear(). Diese Methode wird 12 Monate später seit Dezember 2021 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodRemoveExternalLinksDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Daten für den Kontext hinzu
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Rufen Sie die Methode RemoveExternalLinks auf
                workbook.RemoveExternalLinks();

                // Ergebnisse oder Auswirkungen des Methodenaufrufs anzeigen
                Console.WriteLine("RemoveExternalLinks method called successfully");

                // Speichern Sie die Arbeitsmappe, wenn Änderungen vorgenommen wurden.
                workbook.Save("RemoveExternalLinksDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling RemoveExternalLinks: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


