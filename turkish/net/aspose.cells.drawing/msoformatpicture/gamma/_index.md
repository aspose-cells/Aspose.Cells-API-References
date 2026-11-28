---
title: "MsoFormatPicture.Gamma"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MsoFormatPicture özelliği. Resmin gamasını temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/msoformatpicture/gamma/
---
## MsoFormatPicture.Gamma property

Resmin gamasını temsil eder.

```csharp
public double Gamma { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyGammaDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir resim ekleyin (örnek bir görüntü yolu kullanarak)
            int pictureIndex = sheet.Pictures.Add(5, 5, "sample.jpg");
            Picture picture = sheet.Pictures[pictureIndex];

            // MsoFormatPicture nesnesine erişin
            MsoFormatPicture formatPicture = picture.FormatPicture;

            // Gamma özelliğini ayarla
            formatPicture.Gamma = 1.5; // Demonstrating Gamma adjustment

            // Çalışma kitabını kaydedin
            workbook.Save("MsoFormatPictureGammaDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


