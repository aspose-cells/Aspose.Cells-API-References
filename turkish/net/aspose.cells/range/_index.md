---
title: "Sınıf Range"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Range sınıfı. Bir elektronik tablo içinde hücre aralığını temsil eden nesneyi kapsüller"
type: docs
url: /tr/net/aspose.cells/range/
---
## Range class

Bir elektronik tablo içinde hücre aralığını temsil eden nesneyi kapsar.

```csharp
public class Range : IEnumerable
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [Range](range/#constructor)(CellArea, Cells) | Sınıf yapıcı. |
| [Range](range/#constructor_1)(int, int, int, int, Cells) | Sınıf yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Address](../../aspose.cells/range/address/) { get; } | Aralığın adresini alır. |
| [ColumnCount](../../aspose.cells/range/columncount/) { get; } | Aralıktaki sütun sayısını alır. |
| [ColumnWidth](../../aspose.cells/range/columnwidth/) { get; set; } | Bu aralığın sütun genişliğini ayarlar veya alır |
| [CurrentRegion](../../aspose.cells/range/currentregion/) { get; } | Mevcut bölgeyi temsil eden bir Range nesnesi döndürür. Mevcut bölge, boş satır ve boş sütunların herhangi bir kombinasyonu ile sınırlanan bir aralıktır. |
| [EntireColumn](../../aspose.cells/range/entirecolumn/) { get; } | Belirtilen aralığı içeren tüm sütunu (veya sütunları) temsil eden bir Range nesnesi alır. |
| [EntireRow](../../aspose.cells/range/entirerow/) { get; } | Belirtilen aralığı içeren tüm satırı (veya satırları) temsil eden bir Range nesnesi alır. |
| [FirstColumn](../../aspose.cells/range/firstcolumn/) { get; } | Aralığın ilk sütununun indeksini alır. |
| [FirstRow](../../aspose.cells/range/firstrow/) { get; } | Aralığın ilk satırının indeksini alır. |
| [Height](../../aspose.cells/range/height/) { get; } | Bir aralığın genişliğini nokta cinsinden alır. |
| [Hyperlinks](../../aspose.cells/range/hyperlinks/) { get; } | Aralıktaki tüm köprüleri alır. |
| [Item](../../aspose.cells/range/item/) { get; } | Bu aralıktaki [`Cell`](../cell/) nesnesini alır. |
| [Left](../../aspose.cells/range/left/) { get; } | A sütununun sol kenarından aralığın sol kenarına kadar olan mesafeyi, nokta cinsinden alır. |
| [Name](../../aspose.cells/range/name/) { get; set; } | Aralığın adını alır veya ayarlar. |
| [RefersTo](../../aspose.cells/range/refersto/) { get; } | Aralığın referansını alır. |
| [RowCount](../../aspose.cells/range/rowcount/) { get; } | Aralıktaki satır sayısını alır. |
| [RowHeight](../../aspose.cells/range/rowheight/) { get; set; } | Bu aralıktaki satırların yüksekliğini ayarlar veya alır |
| [Top](../../aspose.cells/range/top/) { get; } | 1. satırın üst kenarından aralığın üst kenarına kadar olan mesafeyi, nokta cinsinden alır. |
| [Value](../../aspose.cells/range/value/) { get; set; } | Aralığın değerini alır ve ayarlar. |
| [Width](../../aspose.cells/range/width/) { get; } | Bir aralığın genişliğini nokta cinsinden alır. |
| [Worksheet](../../aspose.cells/range/worksheet/) { get; } | Bu aralığı içeren [`Worksheet`](./worksheet/) nesnesini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [AddHyperlink](../../aspose.cells/range/addhyperlink/)(string, string, string) | Belirtilen bir hücreye veya hücre aralığına bir hyperlink ekler. |
| [ApplyStyle](../../aspose.cells/range/applystyle/)(Style, StyleFlag) | Tüm bir aralık için biçimlendirmeleri uygular |
| [AutoFill](../../aspose.cells/range/autofill/#autofill)(Range) | Hedef aralığı otomatik olarak doldurur |
| [AutoFill](../../aspose.cells/range/autofill/#autofill_1)(Range, AutoFillType) | Hedef aralığı otomatik olarak doldurur |
| [Clear](../../aspose.cells/range/clear/)() | Bu aralığı temizler. |
| [ClearComments](../../aspose.cells/range/clearcomments/)() | Bu aralığın yorumlarını temizler. |
| [ClearContents](../../aspose.cells/range/clearcontents/)() | Bu aralığın içeriğini temizler. |
| [ClearFormats](../../aspose.cells/range/clearformats/)() | Bu aralığın biçimlerini temizler. |
| [ClearHyperlinks](../../aspose.cells/range/clearhyperlinks/)(bool) | Yalnızca köprüleri kaldırır. |
| [Copy](../../aspose.cells/range/copy/#copy)(Range) | Kaynak bir aralıktan veri (formüller dahil), biçimlendirme, çizim nesneleri vb. kopyalar. |
| [Copy](../../aspose.cells/range/copy/#copy_1)(Range, PasteOptions) | Aralığı özel yapıştırma seçenekleriyle kopyalama. |
| [CopyData](../../aspose.cells/range/copydata/)(Range) | Kaynak bir aralıktan hücre verisini (formüller dahil) kopyalar. |
| [CopyStyle](../../aspose.cells/range/copystyle/)(Range) | Kaynak bir aralıktan stil ayarlarını kopyalar. |
| [CopyValue](../../aspose.cells/range/copyvalue/)(Range) | Kaynak bir aralıktan hücre değerini kopyalar. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable/#exportdatatable)() | Bu aralıktaki verileri bir DataTable nesnesine dışa aktarır. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable/#exportdatatable_1)(ExportTableOptions) | Bu aralıktaki verileri bir DataTable nesnesine dışa aktarır. |
| [ExportDataTableAsString](../../aspose.cells/range/exportdatatableasstring/)() | Bu aralıktaki verileri bir DataTable nesnesine dışa aktarır. |
| [GetCellOrNull](../../aspose.cells/range/getcellornull/)(int, int) | Bu aralıktaki [`Cell`](../cell/) nesnesini veya null değerini alır. |
| [GetEnumerator](../../aspose.cells/range/getenumerator/)() | Bu Range içindeki hücreler için yineleyiciyi alır. |
| [GetOffset](../../aspose.cells/range/getoffset/)(int, int) | `Range` aralığını ofset ile alır. |
| [Intersect](../../aspose.cells/range/intersect/)(Range) | İki aralığın dikdörtgen kesişimini temsil eden bir `Range` nesnesi döndürür. |
| [IsBlank](../../aspose.cells/range/isblank/)() | Aralığın değer içerip içermediğini gösterir. |
| [IsIntersect](../../aspose.cells/range/isintersect/)(Range) | Aralığın kesişip kesişmediğini gösterir. |
| [Merge](../../aspose.cells/range/merge/)() | Bir hücre aralığını tek bir hücreye birleştirir. |
| [MoveTo](../../aspose.cells/range/moveto/)(int, int) | Geçerli aralığı hedef aralığa taşı. |
| [PutValue](../../aspose.cells/range/putvalue/)(string, bool, bool) | Bir değeri aralığa koyar, uygun olduğunda değer başka bir veri tipine dönüştürülür ve hücrenin sayı biçimi sıfırlanır. |
| [SetInsideBorders](../../aspose.cells/range/setinsideborders/)(BorderType, CellBorderType, CellsColor) | Aralığın iç kenarlıklarını ayarla. |
| [SetOutlineBorder](../../aspose.cells/range/setoutlineborder/#setoutlineborder)(BorderType, CellBorderType, CellsColor) | Hücre aralığının etrafına dış kenarlık ayarlar. |
| [SetOutlineBorder](../../aspose.cells/range/setoutlineborder/#setoutlineborder_1)(BorderType, CellBorderType, Color) | Hücre aralığının etrafına dış kenarlık ayarlar. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders/#setoutlineborders)(CellBorderType, CellsColor) | Hücre aralığının etrafındaki dış kenarlıkları aynı kenarlık stili ve rengiyle ayarlar. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders/#setoutlineborders_1)(CellBorderType, Color) | Hücre aralığının etrafındaki dış kenarlıkları aynı kenarlık stili ve rengiyle ayarlar. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders/#setoutlineborders_2)(CellBorderType[], Color[]) | Hücre aralığının etrafına dış kenarlıklar ayarlar. |
| [SetStyle](../../aspose.cells/range/setstyle/#setstyle)(Style) | Aralığın stilini ayarlar. |
| [SetStyle](../../aspose.cells/range/setstyle/#setstyle_1)(Style, bool) | Hücre stilini uygula. |
| [ToHtml](../../aspose.cells/range/tohtml/)(HtmlSaveOptions) | Aralığı html'ye dönüştür. |
| [ToImage](../../aspose.cells/range/toimage/)(ImageOrPrintOptions) | Aralığı görüntüye dönüştürür. |
| [ToJson](../../aspose.cells/range/tojson/)(JsonSaveOptions) | Aralığı JSON değerine dönüştür. |
| override [ToString](../../aspose.cells/range/tostring/)() | Geçerli Range nesnesini temsil eden bir dize döndürür. |
| [Transpose](../../aspose.cells/range/transpose/)() | Verileri satırlardan sütunlara veya tersine (döndür) transpoze et. |
| [Union](../../aspose.cells/range/union/)(Range) | (**Eski.**) İki aralığın birleşimini döndürür. |
| [UnionRang](../../aspose.cells/range/unionrang/)(Range) | (**Eski.**) İki aralığın birleşim sonucunu döndürür. |
| [UnionRanges](../../aspose.cells/range/unionranges/)(Range[]) | İki aralığın birleşim sonucunu döndürür. |
| [UnMerge](../../aspose.cells/range/unmerge/)() | Bu aralığın birleştirilmiş hücrelerini ayırır. |

### Açıklamalar

Range sınıfı, bir Excel elektronik tablosu bölgesini ifade eder. Bununla, aralığın biçimini ayarlayabilir ve değerini belirleyebilirsiniz. Ayrıca Excel aralığını da kolayca kopyalayabilirsiniz.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = cells.CreateRange("A1", "D3");
            range.Value = "Hello";
            workbook.Save("book1.xlsm");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


