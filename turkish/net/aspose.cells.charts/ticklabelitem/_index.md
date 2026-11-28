---
title: "Sınıf TickLabelItem"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.TickLabelItem sınıfı. Grafikte bir işaret etiketi temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/ticklabelitem/
---
## TickLabelItem class

Grafikte bir işaret etiketi temsil eder.

```csharp
public class TickLabelItem
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Height](../../aspose.cells.charts/ticklabelitem/height/) { get; } | Ticklabel öğesinin yüksekliği, grafik yüksekliğinin oranı olarak. |
| [Width](../../aspose.cells.charts/ticklabelitem/width/) { get; } | Ticklabel öğesinin genişliği, grafik genişliğinin oranı olarak. |
| [X](../../aspose.cells.charts/ticklabelitem/x/) { get; } | Ticklabel öğesinin X koordinatları, grafik genişliğinin oranı olarak. |
| [Y](../../aspose.cells.charts/ticklabelitem/y/) { get; } | Ticklabel öğesinin Y koordinatları, grafik yüksekliğinin oranı olarak. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartsClassTickLabelItemDemo
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

            // Bir sütun grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Grafiği hesapla
            chart.Calculate();

            // Kategori ekseni işaret etiketlerine eriş
            Axis axis = chart.CategoryAxis;
            TickLabelItem[] tickLabelItems = axis.TickLabels.TickLabelItems;

            // Her işaret etiketi konumunu işaretlemek için şekiller ekle
            foreach (TickLabelItem item in tickLabelItems)
            {
                // İşaret etiketinin etrafına dikdörtgen ekle
                Shape rectangle = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle,
                    PlacementType.Move,
                    item.X,
                    item.Y,
                    item.X + item.Width,
                    item.Y + item.Height);
                rectangle.Fill.SolidFill.Transparency = 1;
                rectangle.Line.SolidFill.Color = Color.Blue;

                // İşaret etiketinin yanına daire ekle
                Shape circle = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Oval,
                    PlacementType.Move,
                    item.X + item.Width,
                    item.Y,
                    item.X + item.Width + item.Height,
                    item.Y + item.Height);
                circle.Fill.SolidFill.Color = Color.Red;
            }

            // Çalışma kitabını kaydedin
            workbook.Save("TickLabelItemDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


