---
title: "ShapeCollection.AddPictureInChart"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Grafiğe bir resim ekler"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/addpictureinchart/
---
## ShapeCollection.AddPictureInChart method

Grafiğe bir resim ekler.

```csharp
public Picture AddPictureInChart(int top, int left, Stream stream, int widthScale, int heightScale)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üst | Int32 | Şeklin sol üst köşeden dikey ofsetini, grafik alanının 1/4000 birimi cinsinden temsil eder. |
| sol | Int32 | Şeklin sol üst köşeden yatay offseti, grafik alanının 1/4000 biriminde temsil eder. |
| akış | Stream | Görüntü verisini içeren akış nesnesi. |
| widthScale | Int32 | Görüntü genişliğinin ölçeği, yüzde olarak. |
| heightScale | Int32 | Görüntü yüksekliğinin ölçeği, yüzde olarak. |

### Dönüş Değeri

Bir Picture nesnesi döndürür.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts; // Added this using directive
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class ShapeCollectionMethodAddPictureInChartWithInt32Int32StreamInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 15, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);
            chart.NSeries.CategoryData = "B1:B3";

            // Görüntü verisiyle bir bellek akışı oluşturun
            byte[] imageData = File.ReadAllBytes("example.jpg");
            MemoryStream stream = new MemoryStream(imageData);

            try
            {
                // Parametrelerle (Int32, Int32, Stream, Int32, Int32) AddPictureInChart metodunu çağırın
                Picture picture = chart.Shapes.AddPictureInChart(100, 100, stream, 50, 50);
                
                Console.WriteLine("Picture added to chart successfully. Original dimensions: " + 
                    $"{picture.OriginalWidth}x{picture.OriginalHeight}");
                
                // Çalışma kitabını kaydedin
                workbook.Save("AddPictureInChartDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddPictureInChart method: {ex.Message}");
            }
            finally
            {
                stream.Dispose();
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


