---
title: "WebExtensionReferenceCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebExtensionReferenceCollection‑egenskap. Hämtar webbutökning med det specifika indexet"
type: docs
url: /sv/net/aspose.cells.webextensions/webextensionreferencecollection/item/
---
## WebExtensionReferenceCollection indexer

Hämtar web extension efter det specifika indexet.

```csharp
public WebExtensionReference this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet. |

### Returvärde

Webbutökningen

### Exempel

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
                // Skapa en ny WebExtensionReferenceCollection
                WebExtensionReferenceCollection references = new WebExtensionReferenceCollection();
                
                // Lägg till en ny web extension-referens
                int index = references.Add();
                
                // Åtkomst till Item‑egenskapen (skrivskyddad) för att hämta referensen på angivet index
                WebExtensionReference reference = references[index];
                
                // Visa information om den hämtade referensen
                Console.WriteLine($"Retrieved web extension reference at index: {index}");
                Console.WriteLine($"Reference type: {reference.GetType().Name}");
                
                // Obs: Item‑egenskapen är skrivskyddad, så vi demonstrerar bara hur man hämtar dess värde
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating Item property: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [WebExtensionReference](../../webextensionreference/)
* class [WebExtensionReferenceCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


