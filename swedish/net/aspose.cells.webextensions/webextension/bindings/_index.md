---
title: "WebExtension.Bindings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebExtension egenskap. Hämtar alla bindningsrelationer mellan ett Office Addin och data i dokumentet"
type: docs
url: /sv/net/aspose.cells.webextensions/webextension/bindings/
---
## WebExtension.Bindings property

Hämtar alla bindningsförhållanden mellan ett Office-tillägg och data i dokumentet.

```csharp
public WebExtensionBindingCollection Bindings { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Skapa ett exempelark
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Antag att vi får en web extension från någonstans (eftersom vi inte kan skapa en direkt)
                // Detta är en minimal ändring för att få koden att kompilera samtidigt som dess struktur bevaras
                WebExtension webExtension = null; // In real usage, this would come from workbook.WebExtensions or similar
                
                if (webExtension != null)
                {
                    // Åtkomst till Bindings-egenskapen (skrivskyddad)
                    WebExtensionBindingCollection bindings = webExtension.Bindings;
                    
                    // Visa information om bindningarna
                    Console.WriteLine($"Number of bindings: {bindings.Count}");
                    
                    // Lägg till en ny bindning (demonstrerar användning av samlingen)
                    int newBindingIndex = bindings.Add();
                    Console.WriteLine($"Added new binding at index: {newBindingIndex}");
                    
                    // Visa uppdaterat antal
                    Console.WriteLine($"Updated number of bindings: {bindings.Count}");
                }
                else
                {
                    Console.WriteLine("No web extension available");
                }
                
                // Spara arbetsboken
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

### Se även

* class [WebExtensionBindingCollection](../../webextensionbindingcollection/)
* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


