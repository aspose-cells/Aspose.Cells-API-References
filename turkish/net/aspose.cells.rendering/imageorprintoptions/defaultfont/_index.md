---
title: "ImageOrPrintOptions.DefaultFont"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImageOrPrintOptions özelliği. Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa pdfimage'de blok olarak görünebilir. MingLiu veya MS Gothic gibi bir DefaultFont ayarlayarak bu karakterleri gösterebilirsiniz. Bu özellik ayarlanmamışsa Aspose.Cells, bu Unicode karakterleri göstermek için sistemin varsayılan yazı tipini kullanır."
type: docs
url: /tr/net/aspose.cells.rendering/imageorprintoptions/defaultfont/
---
## ImageOrPrintOptions.DefaultFont property

Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipi ayarlanmamışsa, pdf ve görüntüde blok olarak görünebilirler. Bu karakterleri göstermek için MingLiu veya MS Gothic gibi bir DefaultFont ayarlayın. Bu özellik ayarlanmamışsa, Aspose.Cells bu Unicode karakterleri göstermek için sistemin varsayılan yazı tipini kullanacaktır.

```csharp
public string DefaultFont { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyDefaultFontDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücreye örnek metin ekle
            worksheet.Cells["A1"].PutValue("Sample Text with Default Font");

            // Görüntü seçeneklerini oluşturun ve varsayılan yazı tipini ayarlayın
            ImageOrPrintOptions imgOptions = new ImageOrPrintOptions
            {
                DefaultFont = "Arial", // Setting default font
                ImageType = ImageType.Png
            };

            // Çalışma sayfasını görüntüye dönüştür
            SheetRender sheetRender = new SheetRender(worksheet, imgOptions);
            sheetRender.ToImage(0, "output.png");

            Console.WriteLine("Image generated with default font setting.");
        }
    }
}
```

### Ayrıca Bakınız

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


