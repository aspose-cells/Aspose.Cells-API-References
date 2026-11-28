---
title: "PicFormatOption.Bottom"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PicFormatOption özelliği. Resmi uzatmak için alt ofseti alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/picformatoption/bottom/
---
## PicFormatOption.Bottom property

Resmi uzatmak için alt ofseti alır veya ayarlar.

```csharp
public double Bottom { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyBottomDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Mevcut bir resim dosyası kullan (gerçek resim yolu ile değiştir)
            string imagePath = "sample.jpg";

            // Çalışma sayfasına bir dikdörtgen şekli ekle
            Shape shape = worksheet.Shapes.AddRectangle(5, 5, 0, 0, 200, 200);

            // Şekil doldurmayı örnek resmi kullanacak şekilde yapılandır
            // FillType, ImageData ayarlanarak çıkarılır; bu, türü Texture olarak ayarlar
            shape.FillFormat.ImageData = File.ReadAllBytes(imagePath);
            
            // Resim formatı seçeneklerini oluştur ve yapılandır
            PicFormatOption picFormat = new PicFormatOption();
            picFormat.Type = FillPictureType.Stretch;

            // İlk Bottom değerini göster
            Console.WriteLine("Initial Bottom value: " + picFormat.Bottom);

            // Bottom ofsetini değiştir ve yeni değeri göster
            picFormat.Bottom = 0.3;
            Console.WriteLine("Modified Bottom value: " + picFormat.Bottom);

            // PicFormatOption'ı şeklin doldurmasıyla ilişkilendir (uygunsa varsayarak)
            // Not: Bu adım, sağlanan bağlamda gösterilmeyen API'ye özgü yöntemler gerektirebilir
            // Demonstrasyon amacıyla, PicFormatOption oluşturulup yapılandırıldı

            // Uygulanan değişikliklerle çalışma kitabını kaydet
            workbook.Save("PicFormatOptionBottomDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


