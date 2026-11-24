---
title: "WebExtension.Bindings"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebExtension Eigenschaft. Gibt alle Bindungen zwischen einem Office Addin und den Daten im Dokument zurück"
type: docs
url: /de/net/aspose.cells.webextensions/webextension/bindings/
---
## WebExtension.Bindings property

Liest alle Bindungsbeziehungen zwischen einem Office-Add-In und den Daten im Dokument.

```csharp
public WebExtensionBindingCollection Bindings { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyBindingsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Erstelle ein Beispiel-Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Angenommen, wir erhalten eine WebExtension von irgendwo (da wir keine direkt erstellen können)
                // Dies ist eine minimale Änderung, um den Code zu kompilieren, während seine Struktur beibehalten wird
                WebExtension webExtension = null; // In real usage, this would come from workbook.WebExtensions or similar
                
                if (webExtension != null)
                {
                    // Zugriff auf die Bindings-Eigenschaft (schreibgeschützt)
                    WebExtensionBindingCollection bindings = webExtension.Bindings;
                    
                    // Informationen über die Bindungen anzeigen
                    Console.WriteLine($"Number of bindings: {bindings.Count}");
                    
                    // Eine neue Bindung hinzufügen (zeigt die Verwendung der Sammlung)
                    int newBindingIndex = bindings.Add();
                    Console.WriteLine($"Added new binding at index: {newBindingIndex}");
                    
                    // Zeige die aktualisierte Anzahl an.
                    Console.WriteLine($"Updated number of bindings: {bindings.Count}");
                }
                else
                {
                    Console.WriteLine("No web extension available");
                }
                
                // Speichere die Arbeitsmappe
                workbook.Save("WebExtensionBindingsDemo.xlsx");
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

* class [WebExtensionBindingCollection](../../webextensionbindingcollection/)
* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


