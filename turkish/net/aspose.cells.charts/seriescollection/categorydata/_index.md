---
title: "SeriesCollection.CategoryData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SeriesCollection özelliği. Kategori ekseni değerlerinin aralığını alır veya ayarlar. d1e10 gibi bir hücre aralığı veya 26810 gibi bir değer dizisi olabilir"
type: docs
url: /tr/net/aspose.cells.charts/seriescollection/categorydata/
---
## SeriesCollection.CategoryData property

Kategori Ekseni değerlerinin aralığını alır veya ayarlar. Bu, hücre aralığı (örneğin "d1:e10") veya değer dizisi (örneğin "{2,6,8,10}") olabilir.

```csharp
public string CategoryData { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionPropertyCategoryDataDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue("Cat " + (i - 1));
                worksheet.Cells["B" + i].PutValue(i * 10);
            }
            
            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("=Sheet1!$B$2:$B$10", true);
            chart.NSeries.CategoryData = "=Sheet1!$A$2:$A$10";
            
            // Çalışma kitabını kaydedin
            workbook.Save("CategoryDataDemo.xlsx");
            
            // CategoryData özelliğini doğrula
            Console.WriteLine("Chart CategoryData: " + chart.NSeries.CategoryData);
        }
    }
}
```

### Ayrıca Bakınız

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


