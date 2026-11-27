---
title: "Klass ContentTypePropertyCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Properties.ContentTypePropertyCollection-klass. En samling av ContentTypeProperty-objekt som representerar ytterligare information"
type: docs
url: /sv/net/aspose.cells.properties/contenttypepropertycollection/
---
## ContentTypePropertyCollection class

En samling av [`ContentTypeProperty`](../contenttypeproperty/) objekt som representerar ytterligare information.

```csharp
public class ContentTypePropertyCollection : CollectionBase<ContentTypeProperty>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.properties/contenttypepropertycollection/item/) { get; } | Hämtar innehållstypsegenskapen efter ett specifikt index. (2 indexerare) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells.properties/contenttypepropertycollection/add/#add)(string, string) | Lägger till information om innehållstypsegenskap. |
| [Add](../../aspose.cells.properties/contenttypepropertycollection/add/#add_1)(string, string, string) | Lägger till information om innehållstypsegenskap. |
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

### Exempel

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
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();

            // Lägg till en ny egenskap i ContentTypePropertyCollection
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");

            // Åtkomst till ContentTypePropertyCollection
            ContentTypePropertyCollection contentTypeProperties = workbook.ContentTypeProperties;

            // Visar antalet egenskaper
            Console.WriteLine("Number of ContentTypeProperties: " + contentTypeProperties.Count);

            // Åtkomst till en specifik egenskap efter index
            ContentTypeProperty property = contentTypeProperties[0];
            Console.WriteLine("Property Name: " + property.Name);
            Console.WriteLine("Property Value: " + property.Value);
            Console.WriteLine("Property Type: " + property.Type);

            // Ändra kapaciteten för samlingen
            contentTypeProperties.Capacity = 10;
            Console.WriteLine("New Capacity: " + contentTypeProperties.Capacity);

            // Spara Excel-filen
            workbook.Save("ContentTypePropertyCollectionExample.xlsx");
            workbook.Save("ContentTypePropertyCollectionExample.pdf");
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ContentTypeProperty](../contenttypeproperty/)
* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


