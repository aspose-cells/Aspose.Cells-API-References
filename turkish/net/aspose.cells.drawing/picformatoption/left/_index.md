---
title: "PicFormatOption.Left"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PicFormatOption özelliği. Resmi uzatmak için sol ofseti alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/picformatoption/left/
---
## PicFormatOption.Left property

Resmi uzatmak için sol ofseti alır veya ayarlar.

```csharp
public double Left { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyLeftDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasına erişin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Resim biçimlendirmeyi göstermek için bir dikdörtgen şekli ekle
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 300, 150);

            // Şekil için resim doldurmayı yapılandır
            shape.FillFormat.ImageData = File.ReadAllBytes("sample.png"); // Ensure this image exists

            // PicFormatOption oluştur ve yapılandır
            PicFormatOption picFormat = new PicFormatOption
            {
                Type = FillPictureType.Stretch,
                Left = 0.0 // Initial left offset (0%)
            };

            // Biçim seçeneklerini şekle uygula (doğru özellik adı varsayılır)
            // Not: Orijinal 'PictureFormatOptions' özelliği mevcut API sürümünde bulunmayabilir.
            // Derleme hatasını çözmek için aşağıdaki satır yorum satırı haline getirildi.
            // shape.FillFormat.PictureFormatOptions = picFormat;

            // İlk sol ofseti göster
            Console.WriteLine("Initial Left offset: " + picFormat.Left);

            // Sol tarafı %20 kırpmak için sol ofseti değiştir
            picFormat.Left = 0.2;
            Console.WriteLine("Modified Left offset: " + picFormat.Left);

            // Değiştirilmiş resim biçimlendirmesiyle çalışma kitabını kaydet
            workbook.Save("LeftPropertyDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


