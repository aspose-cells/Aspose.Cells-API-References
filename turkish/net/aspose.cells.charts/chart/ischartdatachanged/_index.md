---
title: "Chart.IsChartDataChanged"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Chart yöntemi. Bir grafiğin veri kaynağının değişip değişmediğini algılar"
type: docs
url: /tr/net/aspose.cells.charts/chart/ischartdatachanged/
---
## Chart.IsChartDataChanged method

Bir grafiğin veri kaynağının değişip değişmediğini algılar.

```csharp
public bool IsChartDataChanged()
```

### Dönüş Değeri

Grafik değiştiyse true, aksi takdirde false döndürür

### Açıklamalar

Yöntem, grafiği görüntü formatına render etmeden önce grafiğin veri kaynağındaki değişiklikleri algılar. İlk Chart.toImage çağrısında, grafik kaynak verileri (ör. XValuesParseData, ValuesParseData) kaydedilir. Chart.toImage yöntemi tekrar çağrılmadan önce, Chart'ın yeniden render edilmesi gerekip gerekmediğini kontrol etmek için IsChartDataChanged yöntemini çağırın.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodIsChartDataChangedDemo
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
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik veri aralığını ayarla
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Grafik verisinin değişip değişmediğini kontrol edin (başlangıçta false olmalı)
                bool isChanged = chart.IsChartDataChanged();
                Console.WriteLine($"Chart data changed after creation: {isChanged}");

                // Grafik verisini değiştir
                worksheet.Cells["B2"].PutValue(15);

                // Grafik verisinin tekrar değişip değişmediğini kontrol edin
                isChanged = chart.IsChartDataChanged();
                Console.WriteLine($"Chart data changed after modification: {isChanged}");

                // Grafiği hesaplayarak güncelle
                chart.Calculate();

                // Hesaplamadan sonra kontrol edin
                isChanged = chart.IsChartDataChanged();
                Console.WriteLine($"Chart data changed after calculation: {isChanged}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsChartDataChanged method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("ChartMethodIsChartDataChangedDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


