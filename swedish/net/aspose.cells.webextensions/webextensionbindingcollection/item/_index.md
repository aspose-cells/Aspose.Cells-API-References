---
title: "WebExtensionBindingCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WebExtensionBindingCollection‑egenskap. Hämtar webbutökningens bindningsförhållande efter ett specifikt index"
type: docs
url: /sv/net/aspose.cells.webextensions/webextensionbindingcollection/item/
---
## WebExtensionBindingCollection indexer

Hämtar web extension-bindningsförhållandet efter det specifika indexet.

```csharp
public WebExtensionBinding this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet. |

### Returvärde

Webbutökningens bindningsförhållande

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionBindingCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en webbutökningens bindningssamling
            WebExtensionBindingCollection bindingCollection = new WebExtensionBindingCollection();

            // Lägg till en ny bindning i samlingen
            int index = bindingCollection.Add();

            // Åtkomst till bindningen med Item‑egenskapen (skrivskyddad)
            WebExtensionBinding binding = bindingCollection[index];

            // Ange egenskaper på bindningen
            binding.Id = "binding1";
            binding.Type = "Text";
            binding.Appref = "Sheet1!A1";

            // Visa bindningsdetaljerna
            Console.WriteLine("Binding ID: " + binding.Id);
            Console.WriteLine("Binding Type: " + binding.Type);
            Console.WriteLine("Binding AppRef: " + binding.Appref);

            // Ändra bindningen via samlingen
            bindingCollection[index].Id = "modifiedBinding";
            Console.WriteLine("Modified Binding ID: " + bindingCollection[index].Id);

            // Spara arbetsboken
            workbook.Save("WebExtensionBindingDemo.xlsx");
        }
    }
}
```

### Se även

* class [WebExtensionBinding](../../webextensionbinding/)
* class [WebExtensionBindingCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


