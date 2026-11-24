---
title: "WebExtension.Id"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebExtension Eigenschaft. Gibt die eindeutige Kennung der Office Addin-Instanz im aktuellen Dokument zurück und setzt sie"
type: docs
url: /de/net/aspose.cells.webextensions/webextension/id/
---
## WebExtension.Id property

Liest und setzt die eindeutige Kennung der Office-Add-In-Instanz im aktuellen Dokument.

```csharp
public string Id { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyIdDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // WebExtension-Sammlung aus der Arbeitsmappe abrufen
                var webExtensions = workbook.Worksheets.WebExtensions;
                
                // Eine neue WebExtension hinzufügen (dies erstellt sie mit den erforderlichen Parametern)
                int index = webExtensions.Add();
                WebExtension webExtension = webExtensions[index];
                
                // Die Id-Eigenschaft setzen (da sie les- und schreibbar ist)
                webExtension.Id = "SampleAddin123";
                
                // Den aktuellen Wert der Id-Eigenschaft anzeigen
                Console.WriteLine($"WebExtension Id: {webExtension.Id}");
                
                // Die Id-Eigenschaft ändern, um zu demonstrieren, dass sie schreibbar ist
                webExtension.Id = "UpdatedAddin456";
                Console.WriteLine($"Updated WebExtension Id: {webExtension.Id}");
                
                // Speichere die Arbeitsmappe
                workbook.Save("WebExtensionIdDemo.xlsx");
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

* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


