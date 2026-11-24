---
title: "Klasse ContentTypePropertyCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Properties.ContentTypePropertyCollection‑Klasse. Eine Sammlung von ContentTypeProperty‑Objekten, die zusätzliche Informationen darstellen"
type: docs
url: /de/net/aspose.cells.properties/contenttypepropertycollection/
---
## ContentTypePropertyCollection class

Eine Sammlung von [`ContentTypeProperty`](../contenttypeproperty/)‑Objekten, die zusätzliche Informationen darstellen.

```csharp
public class ContentTypePropertyCollection : CollectionBase<ContentTypeProperty>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.properties/contenttypepropertycollection/item/) { get; } | Liest die Content‑Typ‑Eigenschaft anhand des spezifischen Indexes. (2 Indexer) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells.properties/contenttypepropertycollection/add/#add)(string, string) | Fügt Informationen zur Content‑Typ‑Eigenschaft hinzu. |
| [Add](../../aspose.cells.properties/contenttypepropertycollection/add/#add_1)(string, string, string) | Fügt Informationen zur Content‑Typ‑Eigenschaft hinzu. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ContentTypeProperty) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ContentTypeProperty, IComparer&lt;ContentTypeProperty&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ContentTypeProperty, IComparer&lt;ContentTypeProperty&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ContentTypeProperty) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ContentTypeProperty[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ContentTypeProperty[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ContentTypeProperty[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ContentTypeProperty&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ContentTypeProperty&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ContentTypeProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ContentTypeProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ContentTypeProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ContentTypeProperty&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ContentTypeProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ContentTypeProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ContentTypeProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ContentTypeProperty&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ContentTypeProperty) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ContentTypeProperty, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ContentTypeProperty, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ContentTypeProperty) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ContentTypeProperty, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ContentTypeProperty, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class ContentTypePropertyCollectionDemo
    {
        public static void ContentTypePropertyCollectionExample()
        {
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();

            // Eine neue Eigenschaft zur ContentTypePropertyCollection hinzufügen
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");

            // Zugriff auf die ContentTypePropertyCollection
            ContentTypePropertyCollection contentTypeProperties = workbook.ContentTypeProperties;

            // Anzeige der Anzahl der Eigenschaften
            Console.WriteLine("Number of ContentTypeProperties: " + contentTypeProperties.Count);

            // Zugriff auf eine bestimmte Eigenschaft nach Index
            ContentTypeProperty property = contentTypeProperties[0];
            Console.WriteLine("Property Name: " + property.Name);
            Console.WriteLine("Property Value: " + property.Value);
            Console.WriteLine("Property Type: " + property.Type);

            // Ändern der Kapazität der Sammlung
            contentTypeProperties.Capacity = 10;
            Console.WriteLine("New Capacity: " + contentTypeProperties.Capacity);

            // Speichere die Excel-Datei
            workbook.Save("ContentTypePropertyCollectionExample.xlsx");
            workbook.Save("ContentTypePropertyCollectionExample.pdf");
        }
    }
}
```

### Siehe auch

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ContentTypeProperty](../contenttypeproperty/)
* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


