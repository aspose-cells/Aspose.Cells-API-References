---
title: "WebExtensionReferenceCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WebExtensionReferenceCollection-Eigenschaft. Liest die Web-Extension am angegebenen Index"
type: docs
url: /de/net/aspose.cells.webextensions/webextensionreferencecollection/item/
---
## WebExtensionReferenceCollection indexer

Liefert die Web-Extension anhand des angegebenen Index.

```csharp
public WebExtensionReference this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index. |

### Rückgabewert

Die Web-Extension

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionReferenceCollectionPropertyItemDemo
    {
        public static void Run()
        {
            try
            {
                // Eine neue WebExtensionReferenceCollection erstellen
                WebExtensionReferenceCollection references = new WebExtensionReferenceCollection();
                
                // Füge eine neue Web-Extension-Referenz hinzu
                int index = references.Add();
                
                // Auf die Item-Eigenschaft (schreibgeschützt) zugreifen, um die Referenz am angegebenen Index zu erhalten
                WebExtensionReference reference = references[index];
                
                // Informationen über die abgerufene Referenz anzeigen
                Console.WriteLine($"Retrieved web extension reference at index: {index}");
                Console.WriteLine($"Reference type: {reference.GetType().Name}");
                
                // Hinweis: Die Item-Eigenschaft ist schreibgeschützt, daher demonstrieren wir nur das Auslesen ihres Werts
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating Item property: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [WebExtensionReference](../../webextensionreference/)
* class [WebExtensionReferenceCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


