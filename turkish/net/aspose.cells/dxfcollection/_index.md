---
title: "Sınıf DxfCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.DxfCollection sınıfı. Ana farklı biçimlendirme kayıtlarını temsil eder"
type: docs
url: /tr/net/aspose.cells/dxfcollection/
---
## DxfCollection class

Ana farklı biçimlendirme kayıtlarını temsil eder.

```csharp
public class DxfCollection : CollectionBase<Style>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/dxfcollection/item/) { get; } | Belirtilen indeksteki öğeyi alır. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Style) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Style, IComparer&lt;Style&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Style, IComparer&lt;Style&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Style) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Style[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Style[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Style[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Style&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Style&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Style&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Style&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Style&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Style&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Style&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Style&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Style&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Style&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Style) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Style, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Style, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Style) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Style, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Style, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassDxfCollectionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // DxfCollection'a çalışma kitabından erişin
            DxfCollection dxfCollection = workbook.Worksheets.Dxfs;

            // Stilleri çalışma kitabına oluştur ve ekle (DxfCollection'da kullanılabilir olacak)
            Style headerStyle = workbook.CreateStyle();
            headerStyle.Font.Name = "Calibri";
            headerStyle.Font.Size = 14;
            headerStyle.Font.IsBold = true;
            headerStyle.ForegroundColor = System.Drawing.Color.LightGray;
            headerStyle.Pattern = BackgroundType.Solid;

            Style dataStyle = workbook.CreateStyle();
            dataStyle.Font.Name = "Calibri";
            dataStyle.Font.Size = 11;
            dataStyle.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            dataStyle.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

            // Stilleri DxfCollection aracılığıyla erişin
            Console.WriteLine("Number of styles in DxfCollection: " + dxfCollection.Count);
            Console.WriteLine("First style font: " + dxfCollection[0].Font.Name);

            // Stilleri hücrelere uygula
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A1"].SetStyle(dxfCollection[0]);

            worksheet.Cells["A2"].PutValue("Data");
            worksheet.Cells["A2"].SetStyle(dxfCollection[1]);

            // Bir stili DxfCollection aracılığıyla değiştir
            dxfCollection[1].Font.Color = System.Drawing.Color.Blue;
            worksheet.Cells["A3"].PutValue("Modified Data");
            worksheet.Cells["A3"].SetStyle(dxfCollection[1]);

            // Sonucu kaydet
            workbook.Save("CellsClassDxfCollectionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Style](../style/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


