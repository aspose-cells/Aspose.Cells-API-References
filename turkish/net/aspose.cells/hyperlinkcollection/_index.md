---
title: "HyperlinkCollection sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.HyperlinkCollection sınıfı. Hyperlink nesnelerinin bir koleksiyonunu kapsüller"
type: docs
url: /tr/net/aspose.cells/hyperlinkcollection/
---
## HyperlinkCollection class

Kapsüller bir koleksiyon [`Hyperlink`](../hyperlink/) nesnelerinin.

```csharp
public class HyperlinkCollection : CollectionBase<Hyperlink>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/hyperlinkcollection/item/) { get; } | Belirtilen indeksdeki [`Hyperlink`](../hyperlink/) öğesini alır. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.cells/hyperlinkcollection/add/#add_1)(string, int, int, string) | Belirtilen bir hücreye veya hücre aralığına bir hyperlink ekler. |
| [Add](../../aspose.cells/hyperlinkcollection/add/#add)(int, int, int, int, string) | Belirtilen bir hücreye veya hücre aralığına bir hyperlink ekler. |
| [Add](../../aspose.cells/hyperlinkcollection/add/#add_2)(string, string, string, string, string) | Belirtilen bir hücreye veya hücre aralığına bir hyperlink ekler. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Hyperlink) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Hyperlink, IComparer&lt;Hyperlink&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Hyperlink, IComparer&lt;Hyperlink&gt;) |  |
| [Clear](../../aspose.cells/hyperlinkcollection/clear/#clear)() | Tüm hyperlink'leri temizler. (2 yöntem) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Hyperlink) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Hyperlink[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Hyperlink[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Hyperlink[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Hyperlink&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Hyperlink&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Hyperlink&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Hyperlink&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Hyperlink&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Hyperlink&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Hyperlink&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Hyperlink&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Hyperlink&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Hyperlink&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Hyperlink) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Hyperlink, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Hyperlink, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Hyperlink) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Hyperlink, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Hyperlink, int, int) |  |
| [RemoveAt](../../aspose.cells/hyperlinkcollection/removeat/#removeat)(int) | Bu koleksiyonda belirtilen indeksdeki hyperlink'i kaldırır. (2 yöntem) |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HyperlinkCollectionDemo
    {
        public static void HyperlinkCollectionExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();

            // Eklenen yeni çalışma sayfasının referansını, sayfa indeksini geçirerek elde etme
            Worksheet worksheet = workbook.Worksheets[0];

            // Hyperlink'ler koleksiyonunu al
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;

            // \"A1\" hücresine bir URL'ye köprü ekleme
            hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");

            // \"B1\" hücresine bir URL'ye başka bir köprü ekleme
            hyperlinks.Add("B1", 1, 1, "http://www.example.com");

            // Bir hücre aralığıyla köprü ekleme
            hyperlinks.Add("C1", 1, 2, "http://www.test.com");

            // Görüntülenecek belirli bir metin ve ekran ipucu ile köprü ekleme
            hyperlinks.Add("D1", "D2", "http://www.display.com", "Click Here", "Go to Display");

            // İlk köprüyü kaldırma
            hyperlinks.RemoveAt(0);

            // Tüm köprüleri temizleme
            hyperlinks.Clear();

            // Kaydetmeyi göstermek için köprüyü tekrar ekleme
            hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");

            // Excel dosyasını kaydetme
            workbook.Save("HyperlinkCollectionExample.xlsx");
            workbook.Save("HyperlinkCollectionExample.pdf");
            return;
        }
    }
}
```

### Ayrıca Bakınız

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Hyperlink](../hyperlink/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


