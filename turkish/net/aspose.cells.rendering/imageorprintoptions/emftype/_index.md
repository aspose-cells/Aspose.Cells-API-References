---
title: "ImageOrPrintOptions.EmfType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImageOrPrintOptions özelliği. Metafile formatını belirten bir EmfType alır veya ayarlar. Varsayılan değer EmfPlusDual'dir."
type: docs
url: /tr/net/aspose.cells.rendering/imageorprintoptions/emftype/
---
## ImageOrPrintOptions.EmfType property

Metafile formatını belirten bir EmfType alır veya ayarlar. Varsayılan değer EmfPlusDual.

```csharp
public EmfType EmfType { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertyEmfTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A2"].Value = "EMF Type Demo";

            try
            {
                // ImageOrPrintOptions örneği oluşturun
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Görüntü tipini EMF olarak ayarla
                options.ImageType = Aspose.Cells.Drawing.ImageType.Emf;

                // Seçeneklerle SheetRender oluştur
                SheetRender renderer = new SheetRender(worksheet, options);

                // EMF formatında kaydet
                using (MemoryStream stream = new MemoryStream())
                {
                    renderer.ToImage(0, stream);

                    // EmfType özelliği değerini göster
                    Console.WriteLine("EmfType value: " + options.EmfRenderSetting);

                    // EMF dosyasını kaydet
                    File.WriteAllBytes("output.emf", stream.ToArray());
                    Console.WriteLine("EMF file created successfully.");
                }
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

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


