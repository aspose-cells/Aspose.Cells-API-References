---
title: "Class Row"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Row sınıfı. Çalışma sayfasında tek bir satırı temsil eder"
type: docs
url: /tr/net/aspose.cells/row/
---
## Row class

Bir çalışma sayfasındaki tek bir satırı temsil eder.

```csharp
public class Row : IEnumerable
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [FirstCell](../../aspose.cells/row/firstcell/) { get; } | Satırdaki ilk hücre nesnesini alır. |
| [FirstDataCell](../../aspose.cells/row/firstdatacell/) { get; } | Satırdaki ilk boş olmayan hücreyi alır. |
| [GroupLevel](../../aspose.cells/row/grouplevel/) { get; set; } | Satırın grup seviyesini alır. |
| [HasCustomStyle](../../aspose.cells/row/hascustomstyle/) { get; } | Bu satırın özel stil ayarları (varsayılan ayardan ve çalışma kitabından devralınanından farklı) olup olmadığını gösterir. |
| [Height](../../aspose.cells/row/height/) { get; set; } | Satır yüksekliğini Nokta biriminde alır ve ayarlar. |
| [Index](../../aspose.cells/row/index/) { get; } | Bu satırın dizinini alır. |
| [IsBlank](../../aspose.cells/row/isblank/) { get; } | Satırın herhangi bir veri içerip içermediğini gösterir. |
| [IsCollapsed](../../aspose.cells/row/iscollapsed/) { get; set; } | Satırın katlanmış olup olmadığını gösterir. |
| [IsHeightMatched](../../aspose.cells/row/isheightmatched/) { get; set; } | Satır yüksekliğinin çalışma kitabının mevcut varsayılan yazı tipi ayarına uyup uymadığını gösterir. Bu özelliğin true olması ayrıca satır yüksekliğinin kullanıcı tarafından özel bir değer ayarlanmamış "otomatik" olduğunu gösterir. |
| [IsHidden](../../aspose.cells/row/ishidden/) { get; set; } | Satırın gizli olup olmadığını gösterir. |
| [Item](../../aspose.cells/row/item/) { get; } | Hücreyi alır. |
| [LastCell](../../aspose.cells/row/lastcell/) { get; } | Satırdaki son hücre nesnesini alır. |
| [LastDataCell](../../aspose.cells/row/lastdatacell/) { get; } | Satırdaki son boş olmayan hücreyi alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [ApplyStyle](../../aspose.cells/row/applystyle/)(Style, StyleFlag) | Tüm satır için biçimleri uygular. |
| [CopySettings](../../aspose.cells/row/copysettings/)(Row, bool) | Satırın ayarlarını kopyalar, örneğin stil, yükseklik, görünürlük, ... vb. |
| override [Equals](../../aspose.cells/row/equals/#equals_1)(object) | Bu nesnenin başka bir nesneyle aynı satıra referans verip vermediğini kontrol eder. |
| [Equals](../../aspose.cells/row/equals/#equals)(Row) | Bu nesnenin başka bir satır nesnesiyle aynı satıra referans verip vermediğini kontrol eder. |
| [GetCellByIndex](../../aspose.cells/row/getcellbyindex/)(int) | Bu satırın hücre koleksiyonundaki belirli indeksle hücreyi al. |
| [GetCellOrNull](../../aspose.cells/row/getcellornull/)(int) | Belirli indeksteki hücreyi veya null değerini alır. |
| [GetEnumerator](../../aspose.cells/row/getenumerator/#getenumerator)() | Hücre enumeratörünü alır. |
| [GetEnumerator](../../aspose.cells/row/getenumerator/#getenumerator_1)(bool, bool) | Bu satırdaki hücreleri yineleyen bir enumeratör alır. |
| [GetStyle](../../aspose.cells/row/getstyle/)() | Bu satırın stilini alır. |
| [SetStyle](../../aspose.cells/row/setstyle/)(Style) | Bu satırın stilini ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;
    using System.Collections;

    public class RowDemo
    {
        public static void RowExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasının referansını elde etme
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir stil nesnesi oluşturun
            Style style = workbook.CreateStyle();

            // Arka plan rengini Mavi olarak ayarlama.
            style.BackgroundColor = Color.Blue;

            // Ön plan rengini Kırmızı olarak ayarlama.
            style.ForegroundColor = Color.Red;

            // Arka plan deseni ayarlama.
            style.Pattern = BackgroundType.DiagonalStripe;

            // Yeni Stil Bayrağı.
            StyleFlag styleFlag = new StyleFlag();

            // Tüm Stilleri Ayarla.
            styleFlag.All = true;

            // İlk satırı al.
            Row row = worksheet.Cells.Rows[0];

            // İlk satıra stil uygula
            row.ApplyStyle(style, styleFlag);

            // Satır özelliklerini ayarlama
            row.Height = 20.0;
            row.IsHidden = false;
            row.IsCollapsed = false;
            row.GroupLevel = 1;
            row.IsHeightMatched = true;

            // Satırdaki hücrelere erişme
            Cell firstCell = row.FirstCell;
            Cell firstDataCell = row.FirstDataCell;
            Cell lastCell = row.LastCell;
            Cell lastDataCell = row.LastDataCell;

            // Satırın boş olup olmadığını kontrol etme
            bool isBlank = row.IsBlank;

            // Satırın özel stil içerip içermediğini kontrol etme
            bool hasCustomStyle = row.HasCustomStyle;

            // Satırın indeksini alma
            int rowIndex = row.Index;

            // İndeksle bir hücre alma
            Cell cellByIndex = row.GetCellByIndex(0);

            // Satırın stilini alma
            Style rowStyle = row.GetStyle();

            // Satırın stilini ayarlama
            row.SetStyle(rowStyle);

            // Başka bir satırdan ayarları kopyalama
            Row sourceRow = worksheet.Cells.Rows[1];
            row.CopySettings(sourceRow, true);

            // Satırdaki hücreleri dolaşma
            IEnumerator cellEnumerator = row.GetEnumerator();
            while (cellEnumerator.MoveNext())
            {
                Cell cell = (Cell)cellEnumerator.Current;
                Console.WriteLine(cell.Name + ": " + cell.Value);
            }

            // Excel dosyasını kaydetme
            workbook.Save("RowExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


