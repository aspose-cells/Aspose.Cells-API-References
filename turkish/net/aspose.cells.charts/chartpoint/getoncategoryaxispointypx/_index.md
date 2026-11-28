---
title: "ChartPoint.GetOnCategoryAxisPointYPx"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint metodu. Chart.Calculate metodunu çağırdıktan sonra kategori eksenindeki noktanın y koordinatını alır. Yalnızca Area grafiği için geçerlidir."
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/getoncategoryaxispointypx/
---
## ChartPoint.GetOnCategoryAxisPointYPx method

Chart.Calculate() metodunu çağırdıktan sonra kategori eksenindeki noktanın y-koordinatını alır. Yalnızca Area grafiği için geçerlidir.

```csharp
public float GetOnCategoryAxisPointYPx(int index)
```

### Açıklamalar

Alan 2B grafiği: dizin 0'dır. Alan 3B grafiği: dizin 0 veya 1'dir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetOnCategoryAxisPointYPxWithInt32Demo
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

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Area, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Chart veri kaynağını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Tüm konum özelliklerinin hesaplandığından emin olmak için grafiği hesaplayın
            chart.Calculate();

            // İlk seriden ilk grafik noktasını al
            ChartPoint point = chart.NSeries[0].Points[0];

            try
            {
                // GetOnCategoryAxisPointYPx'i indeks 0 ile çağır
                float yPx = point.GetOnCategoryAxisPointYPx(0);
                
                // Sonucu göster
                Console.WriteLine($"Y coordinate of point on category axis: {yPx} pixels");
                
                // Çalışma kitabını kaydedin
                workbook.Save("ChartPointGetOnCategoryAxisPointYPxDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetOnCategoryAxisPointYPx method: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


