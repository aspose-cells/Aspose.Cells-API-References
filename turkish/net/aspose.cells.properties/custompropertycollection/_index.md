---
title: "Sınıf CustomPropertyCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Properties.CustomPropertyCollection sınıfı. Ek bilgi temsil eden CustomProperty nesnelerinin bir koleksiyonu"
type: docs
url: /tr/net/aspose.cells.properties/custompropertycollection/
---
## CustomPropertyCollection class

Ek bilgi temsil eden [`CustomProperty`](../customproperty/) nesnelerinin bir koleksiyonu.

```csharp
public class CustomPropertyCollection : CollectionBase<CustomProperty>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.properties/custompropertycollection/item/) { get; } | Belirli indeksle özel özelliği alır. (2 indeksleyici) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.cells.properties/custompropertycollection/add/)(string, string) | Özel özellik bilgisi ekler. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CustomProperty) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CustomProperty, IComparer&lt;CustomProperty&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, CustomProperty, IComparer&lt;CustomProperty&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(CustomProperty) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CustomProperty[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CustomProperty[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, CustomProperty[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;CustomProperty&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;CustomProperty&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;CustomProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;CustomProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;CustomProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;CustomProperty&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;CustomProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;CustomProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;CustomProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;CustomProperty&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CustomProperty) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CustomProperty, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CustomProperty, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CustomProperty) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CustomProperty, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CustomProperty, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class CustomPropertyCollectionDemo
    {
        public static void CustomPropertyCollectionExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasının CustomPropertyCollection nesnesine erişin
            CustomPropertyCollection customProperties = worksheet.CustomProperties;

            // Özel özellikler ekle
            customProperties.Add("Author", "John Doe");
            customProperties.Add("Version", "1.0");

            // Özel özelliklere eriş ve yazdır
            for (int i = 0; i < customProperties.Count; i++)
            {
                CustomProperty property = customProperties[i];
                Console.WriteLine($"Name: {property.Name}, Value: {property.Value}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("CustomPropertyCollectionExample.xlsx");
            workbook.Save("CustomPropertyCollectionExample.pdf");
            return;
        }
    }
}
```

### Ayrıca Bakınız

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [CustomProperty](../customproperty/)
* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


