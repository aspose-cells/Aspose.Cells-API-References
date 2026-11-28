---
title: "ChartPoint.XValueType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint özelliği. Grafik noktasının X değer tipini alır"
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/xvaluetype/
---
## ChartPoint.XValueType property

Grafik noktasının X değer tipini alır.

```csharp
public CellValueType XValueType { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyXValueTypeDemo
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

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // İlk grafik noktasını al
            ChartPoint point = chart.NSeries[0].Points[0];

            // Mevcut XValueType'ı göster
            Console.WriteLine("Current XValueType: " + point.XValueType);

            // Yeni XValue'yi ayarla (bu, XValueType'ı otomatik olarak güncelleyecektir)
            point.XValue = DateTime.Now; // Changing to DateTime type
            Console.WriteLine("After setting DateTime value, XValueType: " + point.XValueType);

            point.XValue = "New Category"; // Changing to String type
            Console.WriteLine("After setting String value, XValueType: " + point.XValueType);

            point.XValue = 123.45; // Changing to Numeric type
            Console.WriteLine("After setting Numeric value, XValueType: " + point.XValueType);

            // Çalışma kitabını kaydedin
            workbook.Save("ChartPointXValueTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [CellValueType](../../../aspose.cells/cellvaluetype/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


