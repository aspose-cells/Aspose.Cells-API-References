---
title: "AxisBins.ResetOverflow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AxisBins yöntemi. Taşmayı sıfırla"
type: docs
url: /tr/net/aspose.cells.charts/axisbins/resetoverflow/
---
## AxisBins.ResetOverflow method

Taşmayı sıfırla

```csharp
[Obsolete("This is an internal method.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ResetOverflow()
```

### Açıklamalar

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bu, sorun oluşmasını önlemek için dışarıdan çağrılmasına gerek olmayan dahili bir yöntemdir. Bu özellik, Temmuz 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisBinsMethodResetOverflowDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Bir grafik oluştur
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Değer eksenini al
            Axis valueAxis = chart.ValueAxis;

            // Eksen kutularını oluştur
            AxisBins bins = valueAxis.Bins;

            // Taşma değerini ayarla
            bins.Overflow = 25;
            Console.WriteLine($"Overflow before reset: {bins.Overflow}");

            try
            {
                // ResetOverflow yöntemini çağır
                bins.ResetOverflow();
                Console.WriteLine($"Overflow after reset: {bins.Overflow}");
                Console.WriteLine("ResetOverflow method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ResetOverflow method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("AxisBinsMethodResetOverflowDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [AxisBins](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


