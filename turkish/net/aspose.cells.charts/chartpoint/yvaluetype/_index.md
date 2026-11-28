---
title: "ChartPoint.YValueType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint özelliği. Grafik noktasının Y değer tipini alır"
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/yvaluetype/
---
## ChartPoint.YValueType property

Grafik noktasının Y değer tipini alır.

```csharp
public CellValueType YValueType { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyYValueTypeDemo
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
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // İlk serideki ilk grafik noktasını al
            ChartPoint chartPoint = chart.NSeries[0].Points[0];

            // Mevcut YValueType değerini göster
            Console.WriteLine("Current YValueType: " + chartPoint.YValueType);

            // Değişiklikten önce YValue'yi göster
            Console.WriteLine("Current YValue: " + chartPoint.YValue);

            // YValue'yi farklı bir tipe değiştir (tip değişimini göstermek için string)
            chartPoint.YValue = "15"; // This will change the YValueType to IsString

            // Değişiklikten sonra YValueType'ı göster
            Console.WriteLine("New YValueType: " + chartPoint.YValueType);
            Console.WriteLine("New YValue: " + chartPoint.YValue);

            // Çalışma kitabını kaydedin
            workbook.Save("ChartPointPropertyYValueTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [CellValueType](../../../aspose.cells/cellvaluetype/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


