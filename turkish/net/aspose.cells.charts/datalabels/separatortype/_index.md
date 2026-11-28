---
title: "DataLabels.SeparatorType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataLabels özelliği. Grafikteki veri etiketleri için kullanılan ayırıcı tipini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/datalabels/separatortype/
---
## DataLabels.SeparatorType property

Bir grafikteki veri etiketleri için kullanılan ayırıcı türünü alır veya ayarlar.

```csharp
public DataLabelsSeparatorType SeparatorType { get; set; }
```

### Açıklamalar

Özel ayırıcı ayarlamak için, lütfen `SeparatorType` özelliğini Custom olarak ayarlayın ve ardından [`SeparatorValue`](../separatorvalue/) için beklenen değeri belirtin.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertySeparatorTypeDemo
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

            // Veri etiketlerini etkinleştir
            chart.NSeries[0].DataLabels.ShowValue = true;
            chart.NSeries[0].DataLabels.ShowCategoryName = true;
            
            // Ayırıcı tipini ayarla
            chart.NSeries[0].DataLabels.SeparatorType = DataLabelsSeparatorType.Space;

            // Çalışma kitabını kaydedin
            workbook.Save("DataLabelsSeparatorTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [DataLabelsSeparatorType](../../datalabelsseparatortype/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


