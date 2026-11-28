---
title: "Sınıf WebExtensionPropertyCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.WebExtensions.WebExtensionPropertyCollection sınıfı. Web uzantısı özelliklerinin listesini temsil eder."
type: docs
url: /tr/net/aspose.cells.webextensions/webextensionpropertycollection/
---
## WebExtensionPropertyCollection class

Web uzantısı özellikleri listesinin temsilidir.

```csharp
public class WebExtensionPropertyCollection : CollectionBase<WebExtensionProperty>
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [WebExtensionPropertyCollection](webextensionpropertycollection/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.webextensions/webextensionpropertycollection/item/) { get; } | Web uzantısının özelliğini dizine göre alır. (2 indeksleyici) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.cells.webextensions/webextensionpropertycollection/add/)(string, string) | Web uzantısı özelliği ekler. |
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
| [RemoveAt](../../aspose.cells.webextensions/webextensionpropertycollection/removeat/#removeat_1)(string) | Özelliği ada göre kaldırır. |

### Örnekler

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
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // WebExtensionPropertyCollection örneği oluştur.
                WebExtensionPropertyCollection properties = new WebExtensionPropertyCollection();
                
                // Koleksiyona özellikler ekle.
                int index1 = properties.Add("Color", "Blue");
                int index2 = properties.Add("Size", "Medium");
                
                // İndeksleyici kullanarak özelliklere eriş.
                Console.WriteLine("Property 1: {0} = {1}", 
                    properties[index1].Name, properties[index1].Value);
                Console.WriteLine("Property 2: {0} = {1}", 
                    properties[index2].Name, properties[index2].Value);
                
                // Ada göre özelliğe eriş.
                WebExtensionProperty sizeProperty = properties["Size"];
                Console.WriteLine("Accessed by name: Size = {0}", sizeProperty.Value);
                
                // Bir özelliği kaldır.
                properties.RemoveAt("Color");
                Console.WriteLine("After removal - Count: {0}", properties.Count);
                
                // Çalışma kitabını kaydedin
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

### Ayrıca Bakınız

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [WebExtensionProperty](../webextensionproperty/)
* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


