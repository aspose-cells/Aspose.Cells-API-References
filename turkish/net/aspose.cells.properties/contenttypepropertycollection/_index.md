---
title: "Sınıf ContentTypePropertyCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Properties.ContentTypePropertyCollection sınıfı. Ek bilgi temsil eden ContentTypeProperty nesnelerinin bir koleksiyonu"
type: docs
url: /tr/net/aspose.cells.properties/contenttypepropertycollection/
---
## ContentTypePropertyCollection class

Ek bilgi temsil eden [`ContentTypeProperty`](../contenttypeproperty/) nesnelerinin bir koleksiyonu.

```csharp
public class ContentTypePropertyCollection : CollectionBase<ContentTypeProperty>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.properties/contenttypepropertycollection/item/) { get; } | Belirli bir indeksle içerik türü özelliğini alır. (2 indeksleyici) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.cells.properties/contenttypepropertycollection/add/#add)(string, string) | İçerik türü özelliği bilgisi ekler. |
| [Add](../../aspose.cells.properties/contenttypepropertycollection/add/#add_1)(string, string, string) | İçerik türü özelliği bilgisi ekler. |
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

### Örnekler

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
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();

            // ContentTypePropertyCollection'a yeni bir özellik ekle
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");

            // ContentTypePropertyCollection'a erişim
            ContentTypePropertyCollection contentTypeProperties = workbook.ContentTypeProperties;

            // Özellik sayısını gösterme
            Console.WriteLine("Number of ContentTypeProperties: " + contentTypeProperties.Count);

            // İndeksle belirli bir özelliğe erişim
            ContentTypeProperty property = contentTypeProperties[0];
            Console.WriteLine("Property Name: " + property.Name);
            Console.WriteLine("Property Value: " + property.Value);
            Console.WriteLine("Property Type: " + property.Type);

            // Koleksiyonun kapasitesini değiştirme
            contentTypeProperties.Capacity = 10;
            Console.WriteLine("New Capacity: " + contentTypeProperties.Capacity);

            // Excel dosyasını kaydet
            workbook.Save("ContentTypePropertyCollectionExample.xlsx");
            workbook.Save("ContentTypePropertyCollectionExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [ContentTypeProperty](../contenttypeproperty/)
* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


