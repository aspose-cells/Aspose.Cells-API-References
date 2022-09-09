---
title: TextBoxCollection
second_title: Aspose.Cells for .NET API Referansı
description: Bir koleksiyonu kapsüllerTextBox./textbox nesneler.
type: docs
weight: 2820
url: /tr/net/aspose.cells.drawing/textboxcollection/
---
## TextBoxCollection class

Bir koleksiyonu kapsüller[`TextBox`](../textbox) nesneler.

```csharp
public class TextBoxCollection : CollectionBase<TextBox>
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells.drawing/textboxcollection/item) { get; } | [`TextBox`](../textbox) belirtilen dizindeki öğe. (2 indexers) |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [Add](../../aspose.cells.drawing/textboxcollection/add)(int, int, int, int) | Koleksiyona bir metin kutusu ekler. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(TextBox) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(TextBox, IComparer&lt;TextBox&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, TextBox, IComparer&lt;TextBox&gt;) |  |
| [Clear](../../aspose.cells.drawing/textboxcollection/clear#clear)() | Tüm metin kutularını temizleyin. (2 methods) |
| [Contains](../../aspose.cells/collectionbase`1/contains)(TextBox) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(TextBox[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(TextBox[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, TextBox[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;TextBox&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;TextBox&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;TextBox&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;TextBox&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;TextBox&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;TextBox&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;TextBox&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;TextBox&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;TextBox&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;TextBox&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(TextBox) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(TextBox, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(TextBox, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(TextBox) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(TextBox, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(TextBox, int, int) |  |
| [RemoveAt](../../aspose.cells.drawing/textboxcollection/removeat#removeat)(int) | Dosyadan bir metin kutusunu kaldırın. (2 methods) |

### Örnekler

```csharp

[C#]
//Bir Çalışma Kitabı nesnesini başlatma
Workbook workbook = new Workbook();
// toplama nesnesini al
TextBoxCollection textBoxCollection = workbook.Worksheets[0].TextBoxes;
// bir metin kutusu ekle
textBoxCollection.Add(1, 1, 50, 100);
foreach(TextBox tbox in textBoxCollection)
{
    //ne istiyorsan onu yap
}

//işini yap

```

### Ayrıca bakınız

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [TextBox](../textbox)
* ad alanı [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->