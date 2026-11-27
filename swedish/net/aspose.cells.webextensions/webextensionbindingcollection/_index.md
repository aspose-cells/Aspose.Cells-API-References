---
title: "Klass WebExtensionBindingCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.WebExtensions.WebExtensionBindingCollection class. Representerar listan över bindningsförhållanden mellan ett Office-tillägg och data i dokumentet"
type: docs
url: /sv/net/aspose.cells.webextensions/webextensionbindingcollection/
---
## WebExtensionBindingCollection class

Representerar listan över bindningsförhållanden mellan ett Office-tillägg och data i dokumentet.

```csharp
public class WebExtensionBindingCollection : CollectionBase<WebExtensionBinding>
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [WebExtensionBindingCollection](webextensionbindingcollection/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.webextensions/webextensionbindingcollection/item/) { get; } | Hämtar web extension-bindningsförhållandet efter det specifika indexet. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells.webextensions/webextensionbindingcollection/add/)() | Lägger till ett bindningsförhållande mellan ett Office-tillägg och data i dokumentet. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(WebExtensionBinding) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(WebExtensionBinding, IComparer&lt;WebExtensionBinding&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, WebExtensionBinding, IComparer&lt;WebExtensionBinding&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(WebExtensionBinding) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(WebExtensionBinding[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(WebExtensionBinding[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, WebExtensionBinding[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;WebExtensionBinding&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;WebExtensionBinding&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;WebExtensionBinding&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;WebExtensionBinding&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;WebExtensionBinding&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;WebExtensionBinding&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;WebExtensionBinding&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;WebExtensionBinding&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;WebExtensionBinding&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;WebExtensionBinding&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(WebExtensionBinding) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(WebExtensionBinding, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(WebExtensionBinding, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(WebExtensionBinding) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(WebExtensionBinding, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(WebExtensionBinding, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionsClassWebExtensionBindingCollectionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            
            try
            {
                // Skapa en instans av WebExtensionBindingCollection
                WebExtensionBindingCollection bindings = new WebExtensionBindingCollection();
                
                // Lägg till en ny bindning
                int index = bindings.Add();
                
                // Åtkomst till bindningen via indexeraren
                WebExtensionBinding binding = bindings[index];
                
                // Ange egenskaper på bindningen (förutsatt att dessa egenskaper finns baserat på referensexempel)
                binding.Id = "binding1";
                binding.Type = "table";
                binding.Appref = "Sheet1!A1:B5";
                
                // Visa grundläggande information
                Console.WriteLine($"Created binding with ID: {binding.Id}");
                Console.WriteLine($"Total bindings in collection: {bindings.Count}");
                
                // Spara arbetsboken
                workbook.Save("WebExtensionBindingCollectionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with WebExtensionBindingCollection: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [WebExtensionBinding](../webextensionbinding/)
* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


