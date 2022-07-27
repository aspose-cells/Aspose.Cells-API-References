---
title: Range
second_title: Aspose.Cells for .NET API Referansı
description: Bir elektronik tablo içindeki bir hücre aralığını temsil eden nesneyi kapsüller.
type: docs
weight: 5030
url: /tr/net/aspose.cells/range/
---
## Range class

Bir elektronik tablo içindeki bir hücre aralığını temsil eden nesneyi kapsüller.

```csharp
public class Range
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Address](../../aspose.cells/range/address) { get; } | Aralığın adresini alır. |
| [ColumnCount](../../aspose.cells/range/columncount) { get; } | Aralıktaki sütun sayısını alır. |
| [ColumnWidth](../../aspose.cells/range/columnwidth) { get; set; } | Bu aralığın sütun genişliğini ayarlar veya alır |
| [CurrentRegion](../../aspose.cells/range/currentregion) { get; } | Geçerli bölgeyi temsil eden bir Range nesnesi döndürür. Geçerli bölge, herhangi bir boş satır ve boş sütun kombinasyonuyla sınırlanan bir aralıktır. |
| [EntireColumn](../../aspose.cells/range/entirecolumn) { get; } | Belirtilen aralığı içeren tüm sütunu (veya sütunları) temsil eden bir Aralık nesnesi alır. |
| [EntireRow](../../aspose.cells/range/entirerow) { get; } | Belirtilen aralığı içeren tüm satırı (veya satırları) temsil eden bir Range nesnesi alır. |
| [FirstColumn](../../aspose.cells/range/firstcolumn) { get; } | Aralığın ilk sütununun dizinini alır. |
| [FirstRow](../../aspose.cells/range/firstrow) { get; } | Aralığın ilk satırının dizinini alır. |
| [Height](../../aspose.cells/range/height) { get; } | Nokta olarak bir aralığın genişliğini alır. |
| [Hyperlinks](../../aspose.cells/range/hyperlinks) { get; } | Aralıktaki tüm köprüyü alır. |
| [Item](../../aspose.cells/range/item) { get; } | Alır[`Cell`](../cell) bu aralıktaki nesne. |
| [Left](../../aspose.cells/range/left) { get; } | A sütununun sol kenarından aralığın sol kenarına kadar olan mesafeyi nokta olarak alır. |
| [Name](../../aspose.cells/range/name) { get; set; } | Aralığın adını alır veya ayarlar. |
| [RefersTo](../../aspose.cells/range/refersto) { get; } | Aralığın referanslarını alır. |
| [RowCount](../../aspose.cells/range/rowcount) { get; } | Aralıktaki satır sayısını alır. |
| [RowHeight](../../aspose.cells/range/rowheight) { get; set; } | Bu aralıktaki satırların yüksekliğini ayarlar veya alır |
| [Top](../../aspose.cells/range/top) { get; } | 1. satırın üst kenarından aralığın üst kenarına kadar olan mesafeyi nokta olarak alır. |
| [Value](../../aspose.cells/range/value) { get; set; } | Aralığın değerini alır ve ayarlar. |
| [Width](../../aspose.cells/range/width) { get; } | Nokta olarak bir aralığın genişliğini alır. |
| [Worksheet](../../aspose.cells/range/worksheet) { get; } | [`Worksheet`](./worksheet) bu aralığı içeren nesne. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [ApplyStyle](../../aspose.cells/range/applystyle)(Style, StyleFlag) | Tüm aralık için biçimleri uygular. |
| [AutoFill](../../aspose.cells/range/autofill#autofill)(Range) | Hedef aralığı otomatik olarak doldurur. |
| [AutoFill](../../aspose.cells/range/autofill#autofill_1)(Range, AutoFillType) | Hedef aralığı otomatik olarak doldurur. |
| [Copy](../../aspose.cells/range/copy#copy)(Range) | Bir kaynak aralığından verileri (formüller dahil), biçimlendirmeyi, çizim nesnelerini vb. kopyalar. |
| [Copy](../../aspose.cells/range/copy#copy_1)(Range, PasteOptions) | Özel yapıştırma seçenekleriyle aralığı kopyalama. |
| [CopyData](../../aspose.cells/range/copydata)(Range) | Bir kaynak aralığından hücre verilerini (formüller dahil) kopyalar. |
| [CopyStyle](../../aspose.cells/range/copystyle)(Range) | Bir kaynak aralığından stil ayarlarını kopyalar. |
| [CopyValue](../../aspose.cells/range/copyvalue)(Range) | Bir kaynak aralığından hücre değerini kopyalar. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable#exportdatatable)() | Bu aralıktaki verileri birDataTable nesne. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable#exportdatatable_1)(ExportTableOptions) | Bu aralıktaki verileri birDataTable nesne. |
| [ExportDataTableAsString](../../aspose.cells/range/exportdatatableasstring)() | Bu aralıktaki verileri birDataTable nesne. |
| [GetCellOrNull](../../aspose.cells/range/getcellornull)(int, int) | Alır[`Cell`](../cell) bu aralıkta nesne veya boş. |
| [GetEnumerator](../../aspose.cells/range/getenumerator)() | Bu Aralıktaki hücreler için numaralandırıcıyı alır. |
| [GetOffset](../../aspose.cells/range/getoffset)(int, int) | Alır[`Range`](../range) ofset ile aralık. |
| [Intersect](../../aspose.cells/range/intersect)(Range) | Bir döndürür[`Range`](../range) iki aralığın dikdörtgen kesişimini temsil eden nesne. |
| [IsIntersect](../../aspose.cells/range/isintersect)(Range) | Aralığın kesişip kesişmediğini gösterir. |
| [Merge](../../aspose.cells/range/merge)() | Bir hücre aralığını tek bir hücrede birleştirir. |
| [MoveTo](../../aspose.cells/range/moveto)(int, int) | Geçerli aralığı hedef aralığına taşıyın. |
| [PutValue](../../aspose.cells/range/putvalue)(string, bool, bool) | Aralığa bir değer koyar, uygunsa değer başka bir veri türüne dönüştürülür ve hücrenin sayı biçimi sıfırlanır. |
| [SetInsideBorders](../../aspose.cells/range/setinsideborders)(BorderType, CellBorderType, CellsColor) | Aralığın sınırları içinde ayarlayın. |
| [SetOutlineBorder](../../aspose.cells/range/setoutlineborder)(BorderType, CellBorderType, Color) | Bir hücre aralığı etrafındaki anahat kenarlığını ayarlar. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders#setoutlineborders)(CellBorderType, Color) | Aynı kenarlık stili ve rengine sahip bir hücre aralığı etrafındaki anahat kenarlıklarını ayarlar. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders#setoutlineborders_1)(CellBorderType[], Color[]) | Bir hücre aralığı etrafındaki çizgi sınırlarını belirler. |
| [SetStyle](../../aspose.cells/range/setstyle)(Style) | Aralığın stilini ayarlar. |
| override [ToString](../../aspose.cells/range/tostring)() | Geçerli Range nesnesini temsil eden bir dize döndürür. |
| [Union](../../aspose.cells/range/union)(Range) | İki aralığın birleşimini döndürür. |
| [UnMerge](../../aspose.cells/range/unmerge)() | Bu aralığın birleştirilmiş hücrelerini kaldırır. |

### Örnekler

```csharp

[C#]

//Bir Çalışma Kitabı nesnesini başlatma
Workbook workbook = new Workbook();
// İlk Çalışma Sayfası Hücrelerini alın.
Cells cells = workbook.Worksheets[0].Cells;
// Bir aralık oluşturun (A1:D3).
Range range = cells.CreateRange("A1", "D3");
// Değeri aralığa ayarlayın.
range.Value = "Hello";
//Excel dosyasını kaydedin
workbook.Save("book1.xlsm");

 [Visual Basic]

'Bir Çalışma Kitabı nesnesini başlatma
Dim workbook As Workbook = New Workbook()
'İlk Çalışma Sayfası Hücrelerini alın.
Dim cells as Cells = workbook.Worksheets[0].Cells
'Bir aralık oluşturun (A1:D3).
Dim range as Range = cells.CreateRange("A1", "D3")
'Değeri aralığa ayarlayın.
range.Value = "Hello"
'Excel dosyasını kaydedin
workbook.Save("book1.xlsm")
```

### Ayrıca bakınız

* ad alanı [Aspose.Cells](../../aspose.cells)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
