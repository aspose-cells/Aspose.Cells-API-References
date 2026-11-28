---
title: "ImageOrPrintOptions.Transparent"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImageOrPrintOptions özelliği. Oluşturulan görüntünün arka planının şeffaf olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.rendering/imageorprintoptions/transparent/
---
## ImageOrPrintOptions.Transparent property

Oluşturulan görüntünün arka planının şeffaf olup olmadığını gösterir.

```csharp
public bool Transparent { get; set; }
```

### Açıklamalar

Varsayılan değer false'tur. Bu, oluşturulan görüntülerin arka planının beyaz olduğu anlamına gelir.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyTransparentDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Transparent Image Demo");
            
            // Şeffaf PNG görüntüsüyle HTML kaydetme seçeneklerini ayarla
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ImageOptions.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.ImageOptions.Transparent = true;
            options.ExportImagesAsBase64 = true;

            // Çalışma kitabını şeffaf görüntü seçenekleriyle kaydet
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML with transparent images saved successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


