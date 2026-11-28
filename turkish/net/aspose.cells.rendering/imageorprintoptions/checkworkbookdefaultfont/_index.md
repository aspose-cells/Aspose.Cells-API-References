---
title: "ImageOrPrintOptions.CheckWorkbookDefaultFont"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImageOrPrintOptions özelliği. Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, pdfimage'de blok olarak görünebilirler. Bu özelliği true olarak ayarlayarak, bu karakterleri göstermek için önce çalışma kitabının varsayılan yazı tipini kullanmayı deneyin."
type: docs
url: /tr/net/aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont/
---
## ImageOrPrintOptions.CheckWorkbookDefaultFont property

Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, pdf, görüntüde blok olarak görünebilirler. Bu değeri true olarak ayarlayın, böylece önce çalışma kitabının varsayılan yazı tipini kullanarak bu karakterleri göstermeye çalışır.

```csharp
public bool CheckWorkbookDefaultFont { get; set; }
```

### Açıklamalar

Varsayılan true'dur.

### Örnekler

```csharp
using System;
using System.IO;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyCheckWorkbookDefaultFontDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            sheet.Cells["A1"].PutValue("Sample Text");
            
            // Çalışma kitabı için varsayılan yazı tipini ayarlayın
            workbook.DefaultStyle.Font.Name = "Arial";
            workbook.DefaultStyle.Font.Size = 12;

            // Görüntü veya yazdırma seçenekleri oluştur
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnePagePerSheet = true;
            
            // Çalışma kitabının varsayılan yazı tipini kontrol etmeyi etkinleştirin
            options.CheckWorkbookDefaultFont = true;

            // Çalışma sayfasını görüntüye dönüştür
            SheetRender renderer = new SheetRender(sheet, options);
            using (MemoryStream stream = new MemoryStream())
            {
                renderer.ToImage(0, stream);
                
                // Görüntüyü dosyaya kaydet
                using (FileStream file = new FileStream("output.png", FileMode.Create))
                {
                    stream.WriteTo(file);
                }
            }
            
            Console.WriteLine("Image generated with workbook default font check.");
        }
    }
}
```

### Ayrıca Bakınız

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


