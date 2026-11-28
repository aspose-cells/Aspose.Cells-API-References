---
title: "PicFormatOption.Right"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PicFormatOption özelliği. Resmi uzatmak için sağ ofseti alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/picformatoption/right/
---
## PicFormatOption.Right property

Resmi uzatmak için sağ ofseti alır veya ayarlar.

```csharp
public double Right { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyRightDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasına erişin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Belirtilen boyutlarla bir dikdörtgen şekli ekle
            Shape shape = worksheet.Shapes.AddRectangle(5, 2, 10, 10, 150, 300);

            // Şekil için resim doldurmayı yapılandır
            shape.Fill.FillType = FillType.Texture;
            string imagePath = "sample.jpg"; // Replace with actual image path
            
            if (File.Exists(imagePath))
            {
                shape.Fill.ImageData = File.ReadAllBytes(imagePath);
            }
            else
            {
                Console.WriteLine("Image not found - using empty picture fill");
            }

            // TextureFill aracılığıyla resim format seçeneklerine eriş
            PicFormatOption picFormat = shape.Fill.TextureFill.PicFormatOption;

            // Right özelliğini göster ve değiştir
            Console.WriteLine("Initial Right offset: " + picFormat.Right);
            picFormat.Right = 25.5; // Set right offset to 25.5 units

            // Yeni değeri doğrula ve değişiklikleri kaydet
            Console.WriteLine("Updated Right offset: " + picFormat.Right);
            workbook.Save("RightPropertyDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


