---
title: HyperlinkCollection
second_title: Aspose.Cells for .NET API Referansı
description: Bir koleksiyonu kapsüllerHyperlink./hyperlink nesneler.
type: docs
weight: 3760
url: /tr/net/aspose.cells/hyperlinkcollection/
---
## HyperlinkCollection class

Bir koleksiyonu kapsüller[`Hyperlink`](../hyperlink) nesneler.

```csharp
public class HyperlinkCollection : CollectionBase<Hyperlink>
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells/hyperlinkcollection/item) { get; } | [`Hyperlink`](../hyperlink) belirtilen dizindeki öğe. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [Add](../../aspose.cells/hyperlinkcollection/add#add_1)(string, int, int, string) | Belirtilen hücreye veya hücre aralığına bir köprü ekler. |
| [Add](../../aspose.cells/hyperlinkcollection/add#add)(int, int, int, int, string) | Belirtilen hücreye veya hücre aralığına bir köprü ekler. |
| [Add](../../aspose.cells/hyperlinkcollection/add#add_2)(string, string, string, string, string) | Belirtilen hücreye veya hücre aralığına bir köprü ekler. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Hyperlink) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Hyperlink, IComparer&lt;Hyperlink&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Hyperlink, IComparer&lt;Hyperlink&gt;) |  |
| [Clear](../../aspose.cells/hyperlinkcollection/clear#clear)() | Tüm köprüleri temizler. (2 methods) |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Hyperlink) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Hyperlink[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Hyperlink[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Hyperlink[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Hyperlink&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Hyperlink&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Hyperlink&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Hyperlink&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Hyperlink&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Hyperlink&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Hyperlink&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Hyperlink&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Hyperlink&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Hyperlink&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Hyperlink) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Hyperlink, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Hyperlink, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Hyperlink) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Hyperlink, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Hyperlink, int, int) |  |
| [RemoveAt](../../aspose.cells/hyperlinkcollection/removeat#removeat)(int) | Belirtilen dizindeki köprüyü kaldırın. (2 methods) |

### Örnekler

```csharp


[C#]

//Bir Çalışma Kitabı nesnesini başlatma
Workbook workbook = new Workbook();

//Yeni eklenen çalışma sayfasının sayfa indeksini geçerek referansının alınması
Worksheet worksheet = workbook.Worksheets[0];

//Köprü Koleksiyonunu Al
HyperlinkCollection hyperlinks = worksheet.Hyperlinks;

//"A1" hücresindeki bir URL'ye köprü ekleme
hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");

//Excel dosyasını kaydetme
workbook.Save("book1.xls");

[VB.NET]

'Bir Çalışma Kitabı nesnesini başlatma
Dim workbook As Workbook = New Workbook()

'Yeni eklenen çalışma sayfasının sayfa indeksini geçerek referansını alma
Dim worksheet As Worksheet = workbook.Worksheets(0)

'Köprüler Koleksiyonu Alın
Dim hyperlinks As HyperlinkCollection = worksheet.Hyperlinks

'Adding a hyperlink to a URL at "A1" cell
hyperlinks.Add("A1", 1, 1, "http://www.aspose.com")

'Excel dosyasını kaydetme
workbook.Save("book1.xls")
```

### Ayrıca bakınız

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [Hyperlink](../hyperlink)
* ad alanı [Aspose.Cells](../../aspose.cells)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->