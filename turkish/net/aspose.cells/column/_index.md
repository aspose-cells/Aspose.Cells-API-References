---
title: "Class Column"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Column class. Bir çalışma sayfasındaki tek bir sütunu temsil eder"
type: docs
url: /tr/net/aspose.cells/column/
---
## Column class

Bir çalışma sayfasındaki tek bir sütunu temsil eder.

```csharp
public class Column
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [GroupLevel](../../aspose.cells/column/grouplevel/) { get; set; } | Sütunun grup seviyesini alır. |
| [HasCustomStyle](../../aspose.cells/column/hascustomstyle/) { get; } | Bu sütunun, çalışma kitabından devralınan varsayılan ayardan farklı özel stil ayarlarına sahip olup olmadığını gösterir. |
| [Index](../../aspose.cells/column/index/) { get; } | Bu sütunun dizinini alır. |
| [IsCollapsed](../../aspose.cells/column/iscollapsed/) { get; set; } | sütunun daraltılıp daraltılmadığı |
| [IsHidden](../../aspose.cells/column/ishidden/) { get; set; } | Sütunun gizli olup olmadığını gösterir. |
| [Style](../../aspose.cells/column/style/) { get; } | (**Obsolete.**) Bu sütunun stilini alır. |
| [Width](../../aspose.cells/column/width/) { get; set; } | Sütun genişliğini karakter biriminde alır ve ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [ApplyStyle](../../aspose.cells/column/applystyle/)(Style, StyleFlag) | Tüm bir sütun için biçimleri uygular. |
| [GetStyle](../../aspose.cells/column/getstyle/)() | Bu sütunun stilini alır. |
| [SetStyle](../../aspose.cells/column/setstyle/)(Style) | Bu sütunun stilini ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnDemo
    {
        public static void ColumnExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasının referansını elde etme
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma kitabına yeni Stil ekle
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

            // İlk Sütunu al
            Column column = worksheet.Cells.Columns[0];

            // İlk Sütuna Stili uygula
            column.ApplyStyle(style, styleFlag);

            // Ek özellikler ayarlanıyor
            column.Width = 20.0; // Setting the column width
            column.IsHidden = false; // Setting the column visibility
            column.IsCollapsed = false; // Setting the column collapsed state

            // Excel dosyasını kaydetme
            workbook.Save("ColumnExample.xlsx");
            workbook.Save("ColumnExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


