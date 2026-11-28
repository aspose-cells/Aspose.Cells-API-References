---
title: "ShapePath.WidthPixel"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapePath özelliği. Bu yolun genişliğini piksel biriminde alır"
type: docs
url: /tr/net/aspose.cells.drawing/shapepath/widthpixel/
---
## ShapePath.WidthPixel property

Bu yolun genişliğini piksel biriminde alır.

```csharp
public int WidthPixel { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPropertyWidthPixelDemo
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

                // İlk WidthPixel değerini göster
                Console.WriteLine("Initial WidthPixel value: " + shapePath.WidthPixel);

                // Yeni bir genişlik değeri ayarla
                shapePath.WidthPixel = 300;
                Console.WriteLine("Updated WidthPixel value: " + shapePath.WidthPixel);

                // Şekli çalışma sayfasına ekle
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, shapePath.WidthPixel, 200, new ShapePath[] { shapePath });

                // Çalışma kitabını kaydedin
                workbook.Save("WidthPixelDemo.xlsx");
                Console.WriteLine("WidthPixel property demonstrated successfully.");
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


