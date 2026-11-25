---
title: "Classe WebExtensionPropertyCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.WebExtensions.WebExtensionPropertyCollection. Rappresenta l'elenco delle proprietà dell'estensione web."
type: docs
url: /it/net/aspose.cells.webextensions/webextensionpropertycollection/
---
## WebExtensionPropertyCollection class

Rappresenta l'elenco delle proprietà delle estensioni web.

```csharp
public class WebExtensionPropertyCollection : CollectionBase<WebExtensionProperty>
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [WebExtensionPropertyCollection](webextensionpropertycollection/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.webextensions/webextensionpropertycollection/item/) { get; } | Ottiene la proprietà dell'estensione web per indice. (2 indicizzatori) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells.webextensions/webextensionpropertycollection/add/)(string, string) | Aggiunge una proprietà dell'estensione web. |
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
| [RemoveAt](../../aspose.cells.webextensions/webextensionpropertycollection/removeat/#removeat_1)(string) | Rimuove la proprietà per nome. |

### Esempi

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
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            
            try
            {
                // Crea un'istanza di WebExtensionPropertyCollection
                WebExtensionPropertyCollection properties = new WebExtensionPropertyCollection();
                
                // Aggiunge proprietà alla collezione
                int index1 = properties.Add("Color", "Blue");
                int index2 = properties.Add("Size", "Medium");
                
                // Accede alle proprietà usando l'indicizzatore
                Console.WriteLine("Property 1: {0} = {1}", 
                    properties[index1].Name, properties[index1].Value);
                Console.WriteLine("Property 2: {0} = {1}", 
                    properties[index2].Name, properties[index2].Value);
                
                // Accede alla proprietà per nome
                WebExtensionProperty sizeProperty = properties["Size"];
                Console.WriteLine("Accessed by name: Size = {0}", sizeProperty.Value);
                
                // Rimuove una proprietà
                properties.RemoveAt("Color");
                Console.WriteLine("After removal - Count: {0}", properties.Count);
                
                // Salva la cartella di lavoro
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

### Vedi anche

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [WebExtensionProperty](../webextensionproperty/)
* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


