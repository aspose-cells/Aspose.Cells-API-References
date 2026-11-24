---
title: "WebExtension.AlterReferences"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebExtension Eigenschaft. Gibt eine Liste von Alter‑Referenzen zurück"
type: docs
url: /de/net/aspose.cells.webextensions/webextension/alterreferences/
---
## WebExtension.AlterReferences property

Liest eine Liste von alternativen Verweisen.

```csharp
public WebExtensionReferenceCollection AlterReferences { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyAlterReferencesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // WebExtension-Sammlung aus der Arbeitsmappe abrufen
                var webExtensions = workbook.Worksheets.WebExtensions;
                
                // Füge eine neue Web-Extension hinzu
                int index = webExtensions.Add();
                WebExtension webExtension = webExtensions[index];
                
                // Zugriff auf die AlterReferences‑Eigenschaft (schreibgeschützt)
                WebExtensionReferenceCollection alterReferences = webExtension.AlterReferences;
                
                // Informationen zu den Alter-Referenzen anzeigen
                Console.WriteLine($"Number of alter references: {alterReferences.Count}");
                
                // Füge eine neue Alter-Referenz hinzu (zeigt die Verwendung der Sammlung)
                int newRefIndex = alterReferences.Add();
                Console.WriteLine($"Added new alter reference at index: {newRefIndex}");
                
                // Zeige die aktualisierte Anzahl an.
                Console.WriteLine($"Updated number of alter references: {alterReferences.Count}");
                
                // Speichere die Arbeitsmappe
                workbook.Save("WebExtensionAlterReferencesDemo.xlsx");
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

* class [WebExtensionReferenceCollection](../../webextensionreferencecollection/)
* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


