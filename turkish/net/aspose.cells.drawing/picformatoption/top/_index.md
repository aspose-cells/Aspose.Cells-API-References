---
title: "PicFormatOption.Top"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PicFormatOption özelliği. Resmi uzatmak için üst ofseti alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/picformatoption/top/
---
## PicFormatOption.Top property

Resmi uzatmak için üst ofseti alır veya ayarlar.

```csharp
public double Top { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyTopDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Mevcut bir resmi kullan veya doğru resim yolunu sağla
            string imagePath = "existingImage.png";

            // Doğru parametrelerle bir şekil ekle
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);
            
            // ImageData kullanarak resim doldurmayı uygula
            shape.FillFormat.ImageData = File.ReadAllBytes(imagePath);

            // PicFormatOption'ı doğrudan oluştur ve yapılandır
            PicFormatOption picFormat = new PicFormatOption();

            Console.WriteLine("Initial Top value: " + picFormat.Top);
            picFormat.Top = 0.3;

            // PicFormatOption'ın doldurma formatı ile ilişkilendirilmesi gerektiği varsayılıyor
            // Bu bölüm, tip tanımlarında gösterilmeyen API'ye özgü bir uygulama gerektirebilir
            // shape.FillFormat.SetPicFormatOption(picFormat);

            Console.WriteLine("Modified Top value: " + picFormat.Top);
            workbook.Save("TopPropertyDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


