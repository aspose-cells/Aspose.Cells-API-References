---
title: "TickLabelItem.Y"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TickLabelItem özelliği. Ticklabel öğesinin Y koordinatları, grafik yüksekliğine oran olarak"
type: docs
url: /tr/net/aspose.cells.charts/ticklabelitem/y/
---
## TickLabelItem.Y property

Ticklabel öğesinin Y koordinatları, grafik yüksekliğinin oranı olarak.

```csharp
public double Y { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TickLabelItemPropertyYDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Bir sütun grafik ekle
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B1:B3", true);
            
            // CategoryData yerine NSERIES kullanarak kategori ekseni verilerini ayarla
            chart.NSeries.CategoryData = "A1:A3";

            // Tick etiketlerinin oluşturulmasını sağlamak için grafiği hesapla
            chart.Calculate();

            // Kategori ekseninden tick etiket öğelerini al
            Aspose.Cells.Charts.TickLabelItem[] tickLabelItems = chart.CategoryAxis.TickLabels.TickLabelItems;

            // Y özelliğinin kullanımını, tick etiketleriyle hizalanmış şekiller ekleyerek göster
            for (int i = 0; i < tickLabelItems.Length; i++)
            {
                Aspose.Cells.Charts.TickLabelItem item = tickLabelItems[i];
                
                // Her bir tick etiketinin Y konumuna bir dikdörtgen ekle
                Shape shape = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle, 
                    PlacementType.Move,
                    item.X,
                    item.Y, // Using the Y property of TickLabelItem
                    item.X + 0.05, // Small width
                    item.Y + 0.02); // Small height
                
                shape.Fill.SolidFill.Color = Color.FromArgb(100, 0, 255, 0); // Semi-transparent green
                shape.Line.SolidFill.Color = Color.Black;
            }

            // Çalışma kitabını kaydedin
            workbook.Save("TickLabelItemPropertyYDemo_Output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TickLabelItem](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


