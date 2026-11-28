---
title: "ShapeCollection.AddShapeInChartByScale"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Grafik üzerine bir şekil ekler. Tüm birimler grafik alanının yüzde ölçeğidir"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addshapeinchartbyscale/
---
## AddShapeInChartByScale(MsoDrawingType, PlacementType, double, double, double, double) {#addshapeinchartbyscale}

Grafiğe bir şekil ekle. Tüm birim, grafik alanının yüzde ölçeğidir.

```csharp
public Shape AddShapeInChartByScale(MsoDrawingType type, PlacementType placement, double left, 
    double top, double right, double bottom)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | MsoDrawingType | Çizim türü. |
| yerleştirme | PlacementType | yerleştirme türü. |
| sol | Double | Birim, grafik alanının genişliğinin yüzde ölçeğidir. |
| üst | Double | Birim, grafik alanının yüksekliğinin yüzde ölçeğidir. |
| sağ | Double | Birim, grafik alanının genişliğinin yüzde ölçeğidir. |
| alt | Double | Birim, grafik alanının yüksekliğinin yüzde ölçeğidir. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddShapeInChartByScaleWithMsoDrawingTypePlacementTypeDouDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 1, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Grafiği hesapla
            chart.Calculate();

            // Ölçek koordinatlarını kullanarak grafik üzerine bir dikdörtgen şekli ekleyin
            Shape rectangle = chart.Shapes.AddShapeInChartByScale(
                MsoDrawingType.Rectangle, 
                PlacementType.Move,
                0.2,  // x1 (20% from left)
                0.2,  // y1 (20% from top)
                0.4,  // x2 (40% from left)
                0.4); // y2 (40% from top)
            rectangle.Fill.SolidFill.Color = Color.Blue;
            rectangle.Line.SolidFill.Color = Color.Black;

            // Ölçek koordinatlarını kullanarak grafik üzerine bir oval şekil ekleyin
            Shape oval = chart.Shapes.AddShapeInChartByScale(
                MsoDrawingType.Oval,
                PlacementType.Move,
                0.6,  // x1 (60% from left)
                0.6,  // y1 (60% from top)
                0.8,  // x2 (80% from left)
                0.8); // y2 (80% from top)
            oval.Fill.SolidFill.Color = Color.Red;
            oval.Line.SolidFill.Color = Color.Black;

            // Çalışma kitabını kaydedin
            workbook.Save("AddShapeInChartByScaleWithMsoDrawingType.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* enum [PlacementType](../../placementtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## AddShapeInChartByScale(MsoDrawingType, PlacementType, double, double, double, double, byte[]) {#addshapeinchartbyscale_1}

Grafiğe bir şekil ekle. Tüm birim, grafik alanının 1/4000'idir.

```csharp
public Shape AddShapeInChartByScale(MsoDrawingType type, PlacementType placement, double left, 
    double top, double right, double bottom, byte[] imageData)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | MsoDrawingType | Çizim türü. |
| yerleştirme | PlacementType | yerleştirme türü. |
| sol | Double | Birim, grafik alanının genişliğinin yüzde ölçeğidir. |
| üst | Double | Birim, grafik alanının yüksekliğinin yüzde ölçeğidir. |
| sağ | Double | Birim, grafik alanının genişliğinin yüzde ölçeğidir. |
| alt | Double | Birim, grafik alanının yüksekliğinin yüzde ölçeğidir. |
| imageData | Byte[] | Şekil bir resim veya ole nesnesi değilse, imageData null olmalıdır. |

### Ayrıca Bakınız

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* enum [PlacementType](../../placementtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


