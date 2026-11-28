---
title: "ShapePath.HeightPixel"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapePath özelliği. Bu yolun yüksekliğini piksel biriminde alır"
type: docs
url: /tr/net/aspose.cells.drawing/shapepath/heightpixel/
---
## ShapePath.HeightPixel property

Bu yolun yüksekliğini piksel biriminde alır.

```csharp
public int HeightPixel { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPropertyHeightPixelDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Yeni bir şekil yolu oluştur
                ShapePath shapePath = new ShapePath();

                // Basit bir dikdörtgen yolu oluştur
                shapePath.MoveTo(10, 10);
                shapePath.LineTo(100, 10);
                shapePath.LineTo(100, 50);
                shapePath.LineTo(10, 50);
                shapePath.Close();

                // Mevcut HeightPixel değerini göster
                Console.WriteLine("Initial HeightPixel value: " + shapePath.HeightPixel);

                // Yeni bir yükseklik değeri ayarla
                shapePath.HeightPixel = 200;
                Console.WriteLine("Updated HeightPixel value: " + shapePath.HeightPixel);

                // Şekli çalışma sayfasına ekle
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

                // Çalışma kitabını kaydedin
                workbook.Save("HeightPixelDemo.xlsx");
                Console.WriteLine("HeightPixel property demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


