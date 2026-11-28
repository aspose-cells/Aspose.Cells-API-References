---
title: "Title.Y"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Title özelliği. Grafik alanının 1/4000 biriminde sol üst köşenin y koordinatını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/title/y/
---
## Title.Y property

Sol üst köşenin y koordinatını grafik alanının 1/4000 biriminde alır veya ayarlar.

```csharp
[Obsolete("Use Title.YRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Y { get; set; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine Title.YRatioToChart özelliğini kullanın. Y = YRatioToChart * 4000; Bu özellik Şubat 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TitlePropertyYDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Grafik başlığını ayarla
            chart.Title.Text = "Sample Chart";
            chart.Title.Y = 1000; // Demonstrating Y property - position in 1/4000 units
            
            // Düzenin güncellenmesini sağlamak için grafiği hesapla
            chart.Calculate();

            // Başlığın Y konumuna hizalanmış bir şekil ekle
            Shape shape = chart.Shapes.AddShapeInChart(MsoDrawingType.Rectangle, PlacementType.Move,
                2000, 
                chart.Title.Y, // Using the title's Y property
                3000, 
                chart.Title.Y + 500);
            shape.Fill.SolidFill.Color = Color.Blue;

            // Çalışma kitabını kaydedin
            workbook.Save("TitlePropertyYDemo_Output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


