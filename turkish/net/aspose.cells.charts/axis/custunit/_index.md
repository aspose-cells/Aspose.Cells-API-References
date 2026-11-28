---
title: "Axis.CustUnit"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Axis özelliği. Görüntü birimi için özel bir değer belirtir."
type: docs
url: /tr/net/aspose.cells.charts/axis/custunit/
---
## Axis.CustUnit property

Görüntü birimi için özel bir değer belirtir.

```csharp
[Obsolete("Use Axis.CustomUnit property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int CustUnit { get; set; }
```

### Açıklamalar

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Axis.CustomUnit özelliğini kullanın. Bu özellik, Ocak 2023'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisPropertyCustUnitDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["A5"].PutValue("D");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(1000000);
            worksheet.Cells["B3"].PutValue(2000000);
            worksheet.Cells["B4"].PutValue(3000000);
            worksheet.Cells["B5"].PutValue(4000000);

            // Bir grafik ekleyin ve veri aralığını ayarlayın
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Değer eksenini al
            Axis valueAxis = chart.ValueAxis;

            // Mevcut CustUnit değerini göster (kullanımdan kaldırılmış özellik)
            Console.WriteLine("Current CustUnit value: " + valueAxis.CustUnit);

            // Yeni bir özel birim değeri ayarla (1.000.000)
            valueAxis.CustUnit = 1000000;
            valueAxis.IsDisplayUnitLabelShown = true;

            // Yeni CustUnit değerini göster
            Console.WriteLine("New CustUnit value: " + valueAxis.CustUnit);

            // Sonucu kaydet
            workbook.Save("AxisPropertyCustUnitDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


