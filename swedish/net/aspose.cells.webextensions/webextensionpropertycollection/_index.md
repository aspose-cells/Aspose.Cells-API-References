---
title: "Klass WebExtensionPropertyCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.WebExtensions.WebExtensionPropertyCollection-klass. Representerar listan över web extension‑egenskaper."
type: docs
url: /sv/net/aspose.cells.webextensions/webextensionpropertycollection/
---
## WebExtensionPropertyCollection class

Representerar listan över egenskaper för webbutökning.

```csharp
public class WebExtensionPropertyCollection : CollectionBase<WebExtensionProperty>
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [WebExtensionPropertyCollection](webextensionpropertycollection/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.webextensions/webextensionpropertycollection/item/) { get; } | Hämtar egenskapen för web extension efter index. (2 indexerare) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells.webextensions/webextensionpropertycollection/add/)(string, string) | Lägger till web extension‑egenskap. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(WebExtensionProperty) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(WebExtensionProperty, IComparer&lt;WebExtensionProperty&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, WebExtensionProperty, IComparer&lt;WebExtensionProperty&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(WebExtensionProperty) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(WebExtensionProperty[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(WebExtensionProperty[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, WebExtensionProperty[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;WebExtensionProperty&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;WebExtensionProperty&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;WebExtensionProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;WebExtensionProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;WebExtensionProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;WebExtensionProperty&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;WebExtensionProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;WebExtensionProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;WebExtensionProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;WebExtensionProperty&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(WebExtensionProperty) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(WebExtensionProperty, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(WebExtensionProperty, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(WebExtensionProperty) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(WebExtensionProperty, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(WebExtensionProperty, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
| [RemoveAt](../../aspose.cells.webextensions/webextensionpropertycollection/removeat/#removeat_1)(string) | Ta bort egenskapen efter namn. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionsClassWebExtensionPropertyCollectionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            
            try
            {
                // Skapa en instans av WebExtensionPropertyCollection
                WebExtensionPropertyCollection properties = new WebExtensionPropertyCollection();
                
                // Lägg till egenskaper i samlingen
                int index1 = properties.Add("Color", "Blue");
                int index2 = properties.Add("Size", "Medium");
                
                // Åtkomst till egenskaper med indexerare
                Console.WriteLine("Property 1: {0} = {1}", 
                    properties[index1].Name, properties[index1].Value);
                Console.WriteLine("Property 2: {0} = {1}", 
                    properties[index2].Name, properties[index2].Value);
                
                // Åtkomst till egenskap efter namn
                WebExtensionProperty sizeProperty = properties["Size"];
                Console.WriteLine("Accessed by name: Size = {0}", sizeProperty.Value);
                
                // Ta bort en egenskap
                properties.RemoveAt("Color");
                Console.WriteLine("After removal - Count: {0}", properties.Count);
                
                // Spara arbetsboken
                workbook.Save("WebExtensionPropertyCollectionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with WebExtensionPropertyCollection: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [WebExtensionProperty](../webextensionproperty/)
* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


