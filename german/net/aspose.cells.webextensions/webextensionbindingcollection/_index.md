---
title: "Klasse WebExtensionBindingCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.WebExtensions.WebExtensionBindingCollection-Klasse. Stellt die Liste der Bindungsbeziehungen zwischen einem Office-Add-In und den Daten im Dokument dar."
type: docs
url: /de/net/aspose.cells.webextensions/webextensionbindingcollection/
---
## WebExtensionBindingCollection class

Stellt die Liste der Bindungsbeziehungen zwischen einem Office-Add-In und den Daten im Dokument dar.

```csharp
public class WebExtensionBindingCollection : CollectionBase<WebExtensionBinding>
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [WebExtensionBindingCollection](webextensionbindingcollection/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.webextensions/webextensionbindingcollection/item/) { get; } | Liest die WebExtension-Bindungsbeziehung anhand des angegebenen Index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells.webextensions/webextensionbindingcollection/add/)() | Fügt eine Bindungsbeziehung zwischen einem Office-Add-In und den Daten im Dokument hinzu. |
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

### Beispiele

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
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            
            try
            {
                // Erstelle eine Instanz von WebExtensionBindingCollection
                WebExtensionBindingCollection bindings = new WebExtensionBindingCollection();
                
                // Füge eine neue Bindung hinzu
                int index = bindings.Add();
                
                // Greife über den Indexer auf die Bindung zu
                WebExtensionBinding binding = bindings[index];
                
                // Setze Eigenschaften der Bindung (vorausgesetzt, diese Eigenschaften existieren laut Referenzbeispielen)
                binding.Id = "binding1";
                binding.Type = "table";
                binding.Appref = "Sheet1!A1:B5";
                
                // Zeige grundlegende Informationen an
                Console.WriteLine($"Created binding with ID: {binding.Id}");
                Console.WriteLine($"Total bindings in collection: {bindings.Count}");
                
                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [WebExtensionBinding](../webextensionbinding/)
* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


