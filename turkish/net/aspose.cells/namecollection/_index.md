---
title: "Sınıf NameCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.NameCollection sınıfı. Elektronik tablo içindeki tüm Name nesnelerinin bir koleksiyonunu temsil eder."
type: docs
url: /tr/net/aspose.cells/namecollection/
---
## NameCollection class

Elektronik tabloda bulunan tüm [`Name`](../name/) nesnelerinin bir koleksiyonunu temsil eder.

```csharp
public class NameCollection : CollectionBase<Name>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/namecollection/item/) { get; } | Belirtilen indeksteki [`Name`](../name/) öğesini alır. (2 indeksleyici) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.cells/namecollection/add/)(string) | Yeni bir ad tanımlar. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Name) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Name, IComparer&lt;Name&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Name, IComparer&lt;Name&gt;) |  |
| [Clear](../../aspose.cells/namecollection/clear/#clear)() | Formüller ve veri kaynağı tarafından başvurulmayan tüm tanımlı adları kaldırır. Tanımlı ad başvuruluyorsa, yalnızca Name.ReferTo değerini null olarak ayarlar ve gizleriz. (2 yöntem) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Name) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Name[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Name[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Name[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Name&gt;) |  |
| [Filter](../../aspose.cells/namecollection/filter/)(NameScopeType, int) | Kapsama göre tüm tanımlı adları alır. |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Name&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Name&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Name&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Name&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Name&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Name&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Name&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Name&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Name&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Name) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Name, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Name, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Name) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Name, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Name, int, int) |  |
| [Remove](../../aspose.cells/namecollection/remove/#remove)(string) | İsmi kaldır. |
| [Remove](../../aspose.cells/namecollection/remove/#remove_1)(string[]) | İsim dizisini kaldır. |
| [RemoveAt](../../aspose.cells/namecollection/removeat/#removeat)(int) | Belirli indeksteki ismi kaldır. (2 yöntem) |
| [RemoveDuplicateNames](../../aspose.cells/namecollection/removeduplicatenames/)() | Tanımlı yinelenen isimleri kaldır. |
| [Sort](../../aspose.cells/namecollection/sort/)() | Tanımlı isimleri sıralar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameCollectionDemo
    {
        public static void NameCollectionExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma sayfası koleksiyonuna eriş.
            WorksheetCollection worksheets = workbook.Worksheets;
            
            // İsim koleksiyonuna eriş.
            NameCollection names = worksheets.Names;
            
            // Koleksiyona yeni bir isim ekle.
            int nameIndex = names.Add("MyNamedRange");
            Name name = names[nameIndex];
            
            // İsim için 'refers to' özelliğini ayarla.
            name.RefersTo = "=Sheet1!$A$1:$A$10";
            
            // İsmin özelliklerine eriş ve değiştir.
            name.Comment = "This is a named range for demonstration.";
            name.IsVisible = true;
            
            // Başka bir isim ekle.
            int anotherNameIndex = names.Add("AnotherNamedRange");
            Name anotherName = names[anotherNameIndex];
            anotherName.RefersTo = "=Sheet1!$B$1:$B$10";
            
            // Metne göre bir isim kaldır.
            names.Remove("AnotherNamedRange");
            
            // İndexe göre bir isim kaldır.
            names.RemoveAt(nameIndex);
            
            // Tüm isimleri temizle.
            names.Clear();
            
            // Çalışma kitabını kaydedin
            workbook.Save("NameCollectionExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Name](../name/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


