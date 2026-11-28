---
title: "Sınıf TextTabStopCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.Texts.TextTabStopCollection sınıfı. Tüm sekme duraklarının listesini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing.texts/texttabstopcollection/
---
## TextTabStopCollection class

Tüm sekme duraklarının listesini temsil eder.

```csharp
public class TextTabStopCollection : CollectionBase<TextTabStop>
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [TextTabStopCollection](texttabstopcollection/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.drawing.texts/texttabstopcollection/item/) { get; } | İndeks ile [`TextTabStop`](../texttabstop/) alır. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.cells.drawing.texts/texttabstopcollection/add/)(TextTabAlignmentType, double) | Bir sekme durak ekler. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(TextTabStop) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(TextTabStop, IComparer&lt;TextTabStop&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, TextTabStop, IComparer&lt;TextTabStop&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(TextTabStop) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(TextTabStop[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(TextTabStop[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, TextTabStop[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;TextTabStop&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;TextTabStop&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;TextTabStop&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;TextTabStop&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;TextTabStop&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;TextTabStop&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;TextTabStop&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;TextTabStop&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;TextTabStop&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;TextTabStop&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TextTabStop) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TextTabStop, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TextTabStop, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TextTabStop) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TextTabStop, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TextTabStop, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassTextTabStopCollectionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir metin kutusu şekli oluştur
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 300, 100);
            shape.Text = "Left\tCenter\tRight";

            // Sekme duraklarına erişmek için metin paragrafını al
            var textParagraph = shape.TextBody.TextParagraphs[0];
            var tabStops = textParagraph.Stops;

            // Mevcut sekme duraklarını temizle
            tabStops.Clear();

            // Farklı hizalamalarla sekme durakları ekle
            tabStops.Add(TextTabAlignmentType.Left, 50);
            tabStops.Add(TextTabAlignmentType.Center, 150);
            tabStops.Add(TextTabAlignmentType.Right, 250);

            // Sekme durak bilgilerini göster
            Console.WriteLine("Tab Stops Count: " + tabStops.Count);
            for (int i = 0; i < tabStops.Count; i++)
            {
                Console.WriteLine($"Tab {i}: Position={tabStops[i].TabPosition}, Alignment={tabStops[i].TabAlignment}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("TextTabStopCollectionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [TextTabStop](../texttabstop/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


