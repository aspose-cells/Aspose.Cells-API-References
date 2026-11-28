---
title: "Sınıf CustomXmlPartCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Markup.CustomXmlPartCollection sınıfı. Bir paket içinde Özel XML Veri Depolama Bölümü özel XML verisini temsil eder"
type: docs
url: /tr/net/aspose.cells.markup/customxmlpartcollection/
---
## CustomXmlPartCollection class

Özel bir XML Veri Depolama Bölümünü (paket içindeki özel XML verisi) temsil eder.

```csharp
public class CustomXmlPartCollection : CollectionBase<CustomXmlPart>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.markup/customxmlpartcollection/item/) { get; } | Belirtilen dizindeki bir öğeyi alır. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.cells.markup/customxmlpartcollection/add/)(byte[], byte[]) | Koleksiyona bir öğe ekler. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CustomXmlPart) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CustomXmlPart, IComparer&lt;CustomXmlPart&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, CustomXmlPart, IComparer&lt;CustomXmlPart&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(CustomXmlPart) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CustomXmlPart[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CustomXmlPart[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, CustomXmlPart[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;CustomXmlPart&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;CustomXmlPart&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;CustomXmlPart&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;CustomXmlPart&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;CustomXmlPart&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;CustomXmlPart&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;CustomXmlPart&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;CustomXmlPart&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;CustomXmlPart&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;CustomXmlPart&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CustomXmlPart) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CustomXmlPart, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CustomXmlPart, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CustomXmlPart) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CustomXmlPart, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CustomXmlPart, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
| [SelectByID](../../aspose.cells.markup/customxmlpartcollection/selectbyid/)(string) | Kimliğe göre bir öğeyi alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class MarkupClassCustomXmlPartCollectionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma kitabından CustomXmlPartCollection'ı al
            CustomXmlPartCollection customXmlParts = workbook.CustomXmlParts;

            // Örnek XML verisi ve şeması oluştur
            byte[] xmlData = System.Text.Encoding.UTF8.GetBytes("<root><item>Test</item></root>");
            byte[] schemaData = System.Text.Encoding.UTF8.GetBytes("<xsd:schema xmlns:xsd='http://www.w3.org/2001/XMLSchema'></xsd:schema>");

            // Yeni bir özel XML bölümü ekle
            int index = customXmlParts.Add(xmlData, schemaData);

            // Eklenen XML bölümünü indeks ile al
            CustomXmlPart part = customXmlParts[index];

            // XML bölümünü ID ile seç (biliniyorsa)
            string partId = part.ID;
            CustomXmlPart selectedPart = customXmlParts.SelectByID(partId);

            // Başka bir XML bölümü ekle
            byte[] xmlData2 = System.Text.Encoding.UTF8.GetBytes("<data><value>123</value></data>");
            customXmlParts.Add(xmlData2, null);

            // Özel XML bölümlerinin sayısını göster
            Console.WriteLine("Custom XML parts count: " + customXmlParts.Count);

            // Çalışma kitabını kaydedin
            workbook.Save("CustomXmlPartCollectionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [CustomXmlPart](../customxmlpart/)
* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


