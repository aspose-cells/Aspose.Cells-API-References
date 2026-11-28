---
title: "ShapeCollection.AddAutoShapeInChart"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Bir AutoShape'i çizelgeye ekler"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addautoshapeinchart/
---
## ShapeCollection.AddAutoShapeInChart method

Çarta bir AutoShape ekler.

```csharp
public Shape AddAutoShapeInChart(AutoShapeType type, int top, int left, int height, int width)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | AutoShapeType | Auto şekil türü. |
| üst | Int32 | Metin kutusunun sol üst köşeden dikey ofsetini, çizelge alanının 1/4000 birimi cinsinden temsil eder. |
| sol | Int32 | Metin kutusunun sol üst köşeden dikey ofsetini, çizelge alanının 1/4000 birimi cinsinden temsil eder. |
| yükseklik | Int32 | Metin kutusunun yüksekliğini, çizelge alanının 1/4000 birimi cinsinden temsil eder. |
| genişlik | Int32 | Metin kutusunun genişliğini, çizelge alanının 1/4000 birimi cinsinden temsil eder. |

### Dönüş Değeri

Bir şekil nesnesi döndürür.

### Açıklamalar

Tür, Chart/Comment/Picture/OleObject/Polygon/DialogBox olamaz

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeCollectionMethodAddAutoShapeInChartWithAutoShapeTypeInt32Int32Int32InDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Çizelgeye bir yıldız şekli eklemek için AddAutoShapeInChart yöntemini çağırın
                Shape shape = chart.Shapes.AddAutoShapeInChart(
                    AutoShapeType.Star16,  // AutoShapeType
                    100,                  // Top position (in pixels)
                    100,                  // Left position (in pixels)
                    200,                  // Height (in pixels)
                    200);                 // Width (in pixels)

                // Şekil özelliklerini ayarla
                shape.Name = "SampleStar";
                shape.Fill.SolidFill.Color = System.Drawing.Color.Yellow;
                shape.Line.SolidFill.Color = System.Drawing.Color.Red;

                Console.WriteLine("Star shape added successfully to the chart.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddAutoShapeInChart method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("ShapeCollectionMethodAddAutoShapeInChartDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../../shape/)
* enum [AutoShapeType](../../autoshapetype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


