---
title: "FillFormat.GradientDegree"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FillFormat özelliği. Belirtilen doldurma için gradient derecesini döndürür. Yalnızca Excel 2007 için geçerlidir."
type: docs
url: /tr/net/aspose.cells.drawing/fillformat/gradientdegree/
---
## FillFormat.GradientDegree property

Belirtilen dolgu için gradient derecesini döndürür. Yalnızca Excel 2007 için geçerlidir.

```csharp
public double GradientDegree { get; }
```

### Açıklamalar

0.0 (koyu) ile 1.0 (açık) arasında bir değer olabilir.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyGradientDegreeDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // İlk seri için gradient doldurmayı ayarla
            Aspose.Cells.Drawing.FillFormat fillFormat = chart.NSeries[0].Area.FillFormat;
            fillFormat.SetTwoColorGradient(Color.Red, Color.Blue, Aspose.Cells.Drawing.GradientStyleType.Horizontal, 2);
            
            // Gradient derecesini göster
            Console.WriteLine("Gradient Degree: " + fillFormat.GradientDegree);

            // Çalışma kitabını kaydedin
            workbook.Save("GradientDegreeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


