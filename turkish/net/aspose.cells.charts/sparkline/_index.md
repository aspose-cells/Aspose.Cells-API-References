---
title: "Sınıf Sparkline"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.Sparkline sınıfı. Bir sparkline, bir çalışma sayfası hücresinde veri görselleştirmesi sağlayan küçük bir grafik veya çizelgeyi temsil eder."
type: docs
url: /tr/net/aspose.cells.charts/sparkline/
---
## Sparkline class

Bir sparkline, veri görsel temsili sağlayan bir çalışma sayfası hücresindeki küçük bir grafik veya görseli temsil eder.

```csharp
public class Sparkline
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Column](../../aspose.cells.charts/sparkline/column/) { get; } | Sparkline'ın sütun indeksini alır. |
| [DataRange](../../aspose.cells.charts/sparkline/datarange/) { get; set; } | Sparkline'ın veri aralığını temsil eder. |
| [Row](../../aspose.cells.charts/sparkline/row/) { get; } | Sparkline'ın satır indeksini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [ToImage](../../aspose.cells.charts/sparkline/toimage/#toimage)(ImageOrPrintOptions) | Bir sparkline'ı görüntüye dönüştürür. |
| [ToImage](../../aspose.cells.charts/sparkline/toimage/#toimage_1)(Stream, ImageOrPrintOptions) | Bir sparkline'ı görüntüye dönüştürür. |
| [ToImage](../../aspose.cells.charts/sparkline/toimage/#toimage_2)(string, ImageOrPrintOptions) | Bir sparkline'ı görüntüye dönüştürür. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SparklineDemo
    {
        public static void SparklineExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı veriler ekle
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Sparkline için CellArea'yı tanımla
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Çalışma sayfasına bir sparkline grubu ekle
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, sheet.Name + "!A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Gruba bir sparkline ekle
            idx = group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 5);
            Sparkline line = group.Sparklines[idx];

            // Sparkline ayrıntılarını çıktıla
            Console.WriteLine("Sparkline data range: " + line.DataRange + ", row: " + line.Row + ", column: " + line.Column);

            // Sparkline'ı görüntü olarak kaydet
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = Aspose.Cells.Drawing.ImageType.Png,
                HorizontalResolution = 300,
                VerticalResolution = 300
            };
            line.ToImage("output.png", options);

            // Çalışma kitabını kaydedin
            workbook.Save("SparklineExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


