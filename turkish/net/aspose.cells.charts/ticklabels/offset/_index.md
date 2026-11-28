---
title: "TickLabels.Offset"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TickLabels özelliği. Etiketlerin kategori ekseninden uzaklığını alır ve ayarlar. Bu yalnızca kategori x ekseni için geçerlidir."
type: docs
url: /tr/net/aspose.cells.charts/ticklabels/offset/
---
## TickLabels.Offset property

Etiketlerin kategori ekseninden (x) uzaklığını alır ve ayarlar. Bu yalnızca kategori (x) ekseni için geçerlidir.

```csharp
public int Offset { get; set; }
```

### Açıklamalar

Varsayılan mesafe %100'tür, bu eksen etiketleri ile eksen çizgisi arasındaki varsayılan boşluğu temsil eder. Değer, eksen etiketinin yazı tipi boyutuna göre 0 ile 1000 arasında bir tam sayı yüzde olarak olabilir.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyOffsetDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Bir grafik ekleyin
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Chart veri kaynağını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Değer eksenine erişin
            Axis valueAxis = chart.ValueAxis;
            
            // TickLabels offset'ini ayarla
            valueAxis.TickLabels.Offset = 50; // 50% offset from default position

            // Çalışma kitabını kaydedin
            workbook.Save("TickLabelsOffsetDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


