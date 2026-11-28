---
title: "SeriesCollection.SecondCategoryData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SeriesCollection özelliği. İkinci kategori ekseni değerlerinin aralığını alır veya ayarlar. d1e10 gibi bir hücre aralığı veya 26810 gibi bir değer dizisi olabilir. Yalnızca bazı seriler ikinci eksende çizildiğinde etkili olur"
type: docs
url: /tr/net/aspose.cells.charts/seriescollection/secondcategorydata/
---
## SeriesCollection.SecondCategoryData property

İkinci kategori Ekseni değerlerinin aralığını alır veya ayarlar. Bu, hücre aralığı (örneğin "d1:e10") veya değer dizisi (örneğin "{2,6,8,10}") olabilir. Yalnızca bazı seriler ikinci eksende çizildiğinde etkili olur.

```csharp
public string SecondCategoryData { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionPropertySecondCategoryDataDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Primary Categories");
            worksheet.Cells["A2"].PutValue("Cat1");
            worksheet.Cells["A3"].PutValue("Cat2");
            worksheet.Cells["A4"].PutValue("Cat3");
            
            worksheet.Cells["B1"].PutValue("Secondary Categories");
            worksheet.Cells["B2"].PutValue("SubCat1");
            worksheet.Cells["B3"].PutValue("SubCat2");
            worksheet.Cells["B4"].PutValue("SubCat3");
            
            worksheet.Cells["C1"].PutValue("Values");
            worksheet.Cells["C2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(20);
            worksheet.Cells["C4"].PutValue(30);

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Seri verilerini ayarla
            chart.NSeries.Add("C2:C4", true);
            
            // Birincil kategori verilerini ayarla
            chart.NSeries.CategoryData = "A2:A4";
            
            // İkincil kategori verilerini ayarla
            chart.NSeries.SecondCategoryData = "B2:B4";

            // Çalışma kitabını kaydedin
            workbook.Save("SecondCategoryDataDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


