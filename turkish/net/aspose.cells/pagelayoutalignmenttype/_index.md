---
title: "Enum PageLayoutAlignmentType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.PageLayoutAlignmentType enum. Sayfa düzeni hizalama türlerini listeler"
type: docs
url: /tr/net/aspose.cells/pagelayoutalignmenttype/
---
## PageLayoutAlignmentType enumeration

Sayfa düzeni hizalama türlerini numaralandırır.

```csharp
public enum PageLayoutAlignmentType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Bottom | `0` | Alt sayfa düzeni hizalamasını temsil eder. |
| Center | `1` | Orta sayfa düzeni hizalamasını temsil eder. |
| Left | `2` | Sol sayfa düzeni hizalamasını temsil eder. |
| Right | `3` | Sağ sayfa düzeni hizalamasını temsil eder. |
| Top | `4` | Üst sayfa düzeni hizalamasını temsil eder. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PageLayoutAlignmentTypeDemo
    {
        public static void PageLayoutAlignmentTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı örnek veriler ekleyin
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);
            worksheet.Cells["A4"].PutValue(789);

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Grafik için veri aralığını ayarlayın
            chart.SetChartDataRange("A1:A4", true);

            // Grafiğin başlığını ayarlayın
            chart.Title.Text = "Sample Chart";

            // Çalışma kitabını bir dosyaya kaydedin
            workbook.Save("PageLayoutAlignmentTypeExample.xlsx");

            // Grafiği belirli sayfa düzeni hizalamasıyla PDF'ye dışa aktarın
            chart.ToPdf("ChartExample.pdf", 8.5f, 11f, PageLayoutAlignmentType.Center, PageLayoutAlignmentType.Center);

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


