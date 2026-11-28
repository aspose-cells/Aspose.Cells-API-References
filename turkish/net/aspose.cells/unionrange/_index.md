---
title: "Sınıf UnionRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.UnionRange sınıfı. Birleşik aralığı temsil eder"
type: docs
url: /tr/net/aspose.cells/unionrange/
---
## UnionRange class

Birleşik aralığı temsil eder.

```csharp
public class UnionRange : IEnumerable
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CellCount](../../aspose.cells/unionrange/cellcount/) { get; } | Aralıktaki tüm hücre sayısını alır. |
| [ColumnCount](../../aspose.cells/unionrange/columncount/) { get; } | Aralıktaki satır sayısını alır. |
| [FirstColumn](../../aspose.cells/unionrange/firstcolumn/) { get; } | Aralığın ilk sütununun indeksini alır. |
| [FirstRow](../../aspose.cells/unionrange/firstrow/) { get; } | Aralığın ilk satırının indeksini alır. |
| [HasRange](../../aspose.cells/unionrange/hasrange/) { get; } | Bu öğenin aralığa sahip olup olmadığını gösterir. |
| [Hyperlinks](../../aspose.cells/unionrange/hyperlinks/) { get; } | Aralıktaki tüm köprüleri alır. |
| [Name](../../aspose.cells/unionrange/name/) { get; set; } | Aralığın adını alır veya ayarlar. |
| [RangeCount](../../aspose.cells/unionrange/rangecount/) { get; } | Aralıkların sayısını alır. |
| [Ranges](../../aspose.cells/unionrange/ranges/) { get; } | Tüm birleşim aralıklarını alır. |
| [RefersTo](../../aspose.cells/unionrange/refersto/) { get; } | Aralığın referansını alır. |
| [RowCount](../../aspose.cells/unionrange/rowcount/) { get; } | Aralıktaki satır sayısını alır. |
| [Value](../../aspose.cells/unionrange/value/) { get; set; } | Aralığın değerlerini alır ve ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [ApplyStyle](../../aspose.cells/unionrange/applystyle/)(Style, StyleFlag) | Tüm bir aralık için biçimlendirmeleri uygular |
| [Copy](../../aspose.cells/unionrange/copy/)(UnionRange, PasteOptions) | Aralığı özel yapıştırma seçenekleriyle kopyalama. |
| [GetEnumerator](../../aspose.cells/unionrange/getenumerator/)() | Bu Range içindeki hücreler için yineleyiciyi alır. |
| [Intersect](../../aspose.cells/unionrange/intersect/#intersect)(Range[]) | Başka bir aralıkla kesişir. |
| [Intersect](../../aspose.cells/unionrange/intersect/#intersect_2)(string) | Başka bir aralıkla kesişir. |
| [Intersect](../../aspose.cells/unionrange/intersect/#intersect_1)(UnionRange) | Başka bir aralıkla kesişir. |
| [Merge](../../aspose.cells/unionrange/merge/)() | Bir hücre aralığını tek bir hücreye birleştirir. |
| [PutValue](../../aspose.cells/unionrange/putvalue/)(string, bool, bool) | Bir değeri aralığa koyar, uygun olduğunda değer başka bir veri tipine dönüştürülür ve hücrenin sayı biçimi sıfırlanır. |
| [SetOutlineBorders](../../aspose.cells/unionrange/setoutlineborders/#setoutlineborders)(CellBorderType, Color) | Hücre aralığının etrafındaki dış kenarlıkları aynı kenarlık stili ve rengiyle ayarlar. |
| [SetOutlineBorders](../../aspose.cells/unionrange/setoutlineborders/#setoutlineborders_1)(CellBorderType[], Color[]) | Hücre aralığının etrafına dış kenarlıklar ayarlar. |
| [SetStyle](../../aspose.cells/unionrange/setstyle/)(Style) | Aralığın stilini ayarlar. |
| [Union](../../aspose.cells/unionrange/union/#union)(Range[]) | Aralıkları birleştir. |
| [Union](../../aspose.cells/unionrange/union/#union_2)(string) | Başka bir aralığı birleştir. |
| [Union](../../aspose.cells/unionrange/union/#union_1)(UnionRange) | Başka bir aralığı birleştir. |
| [UnMerge](../../aspose.cells/unionrange/unmerge/)() | Bu aralığın birleştirilmiş hücrelerini ayırır. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassUnionRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Doğru API'yi kullanarak bir birleşim aralığı oluştur.
            UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:A10,C1:C10", 0);
            
            // Tüm birleşim aralığı için değeri ayarla.
            unionRange.Value = "Test";
            
            // Birleşim aralığına stil uygula.
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            unionRange.ApplyStyle(style, new StyleFlag { All = true });
            
            // Çalışma kitabını kaydedin
            workbook.Save("UnionRangeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


