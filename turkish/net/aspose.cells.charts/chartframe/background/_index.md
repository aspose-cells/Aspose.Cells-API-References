---
title: "ChartFrame.Background"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartFrame özelliği. Arka planın görüntüleme modunu alır ve ayarlar. Bu özellik yalnızca Excel 2003 veya daha eski sürümlerde geçerlidir."
type: docs
url: /tr/net/aspose.cells.charts/chartframe/background/
---
## ChartFrame.Background property

Arka planın görüntüleme modunu alır ve ayarlar. Bu özellik yalnızca Excel 2003 veya daha eski sürümlerde geçerlidir.

```csharp
[Obsolete("Use ChartFrame.Area.FillFormat.FillType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public BackgroundMode Background { get; set; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen ChartFrame.Area.FillFormat.FillType özelliğini kullanın. Örneğin, BackgroundMode'u Opaque olarak ayarlamanız gerekiyorsa, aşağıdaki kodu kullanabilirsiniz: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Bu özellik, OCAK 2012'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyBackgroundDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik verilerini yapılandır
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Arka plan ayarlarıyla veri etiketlerini yapılandır
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;
            dataLabels.Background = BackgroundMode.Transparent;

            // Çalışma kitabını kaydedin
            workbook.Save("ChartBackgroundDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [BackgroundMode](../../backgroundmode/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


