---
title: "TickLabelItem.Height"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TickLabelItem özelliği. Ticklabel öğesinin yüksekliği, grafik yüksekliğine oran olarak"
type: docs
url: /tr/net/aspose.cells.charts/ticklabelitem/height/
---
## TickLabelItem.Height property

Ticklabel öğesinin yüksekliği, grafik yüksekliğinin oranı olarak.

```csharp
public double Height { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TickLabelItemPropertyHeightDemo
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

            // Bir sütun grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Grafiği hesapla
            chart.Calculate();

            // Kategori ekseni işaret etiketlerine eriş
            Axis axis = chart.CategoryAxis;
            TickLabelItem[] tickLabelItems = axis.TickLabels.TickLabelItems;

            // Tik etiketi öğesi yüksekliklerini görselleştirmek için şekiller ekle
            foreach (TickLabelItem item in tickLabelItems)
            {
                // Tik etiketi öğesinin sınırlarını gösteren bir dikdörtgen ekle
                Shape shape = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle,
                    PlacementType.Move,
                    item.X,
                    item.Y,
                    item.X + item.Width,
                    item.Y + item.Height);
                
                shape.Fill.SolidFill.Transparency = 1;
                shape.Line.SolidFill.Color = Color.Blue;

                // Yükseklik değerini gösteren metin ekle
                Shape textShape = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.TextBox,
                    PlacementType.Move,
                    item.X,
                    item.Y - 0.05, // Position above the tick label
                    0.1,
                    0.05);
                
                textShape.Text = $"H: {item.Height:F4}";
                textShape.Fill.SolidFill.Transparency = 1;
            }

            // Çalışma kitabını kaydedin
            workbook.Save("TickLabelItemHeightDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TickLabelItem](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


