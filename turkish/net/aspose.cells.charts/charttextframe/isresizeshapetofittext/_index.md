---
title: "ChartTextFrame.IsResizeShapeToFitText"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartTextFrame özelliği. Bir şeklin içinde tanımlanan metni tamamen içerecek şekilde otomatik olarak sığdırılıp sığdırılmayacağını alır veya ayarlar. Otomatik sığdırma, bir şeklin içindeki metnin tüm metni kapsayacak şekilde ölçeklendirilmesidir"
type: docs
url: /tr/net/aspose.cells.charts/charttextframe/isresizeshapetofittext/
---
## ChartTextFrame.IsResizeShapeToFitText property

Bir şeklin içinde tanımlanan metni tamamen içerecek şekilde otomatik olarak sığdırılıp sığdırılmayacağını alır veya ayarlar. Otomatik sığdırma, bir şeklin içindeki metnin tüm metni içerecek şekilde ölçeklendirilmesidir.

```csharp
public bool IsResizeShapeToFitText { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyIsResizeShapeToFitTextDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Bir sütun grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Seri verilerini ayarla
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Veri etiketlerine eriş
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;
            dataLabels.Position = LabelPositionType.Center;

            // IsResizeShapeToFitText özelliğini göster
            foreach (ChartPoint point in chart.NSeries[0].Points)
            {
                // Metni sığdırmak için şeklin otomatik yeniden boyutlandırılmasını devre dışı bırak
                point.DataLabels.IsResizeShapeToFitText = false;
                
                // Metnin normalde gerektireceğinden daha küçük özel bir genişlik ayarla
                point.DataLabels.Width = 50;
            }

            // Çalışma kitabını kaydedin
            workbook.Save("ChartTextFramePropertyIsResizeShapeToFitTextDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


