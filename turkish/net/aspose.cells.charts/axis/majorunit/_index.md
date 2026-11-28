---
title: "Axis.MajorUnit"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Axis özelliği. Eksen için ana birimleri temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/axis/majorunit/
---
## Axis.MajorUnit property

Eksen için ana birimleri temsil eder.

```csharp
public double MajorUnit { get; set; }
```

### Açıklamalar

Ana birimler sıfırdan büyük olmalıdır.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMajorUnitDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Category");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Cat " + i);
                worksheet.Cells["B" + (i + 1)].PutValue(i * 10);
            }

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B11", true);
            chart.NSeries.CategoryData = "A2:A11";

            // Kategori eksenini al
            Axis axis = chart.CategoryAxis;

            // İlk ana birimi göster
            Console.WriteLine("Initial Major Unit: " + axis.MajorUnit);

            // Yeni ana birimi ayarla
            axis.MajorUnit = 3;
            Console.WriteLine("Modified Major Unit: " + axis.MajorUnit);

            // Çalışma kitabını kaydedin
            workbook.Save("AxisMajorUnitDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


