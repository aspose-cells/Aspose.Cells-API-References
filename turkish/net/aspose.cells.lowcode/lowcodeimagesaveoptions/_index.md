---
title: "Sınıf LowCodeImageSaveOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.LowCode.LowCodeImageSaveOptions sınıfı. Düşük kod yöntemiyle görüntü kaydetme seçenekleri"
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodeimagesaveoptions/
---
## LowCodeImageSaveOptions class

Düşük kodlu bir şekilde görüntü kaydetme seçenekleri.

```csharp
public class LowCodeImageSaveOptions : LowCodeSaveOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [LowCodeImageSaveOptions](lowcodeimagesaveoptions/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ImageOptions](../../aspose.cells.lowcode/lowcodeimagesaveoptions/imageoptions/) { get; set; } | Görüntüleri işleme seçenekleri. |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | Oluşturulan verileri kaydetmek için dosyayı (gerekirse yol ile) alır ve ayarlar. Bu özelliği null veya boş dize dışındaki bir değerle ayarladığınızda, [`OutputStream`](../lowcodesaveoptions/outputstream/) yok sayılacaktır. ([`LowCodeSaveOptions`](../lowcodesaveoptions/) sınıfından devralınmıştır.) |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | Oluşturulan verileri yazmak için akışı alır ve ayarlar. Bu özelliği null dışındaki bir değerle ayarladığınızda, [`OutputFile`](../lowcodesaveoptions/outputfile/) yok sayılacaktır. ([`LowCodeSaveOptions`](../lowcodesaveoptions/) sınıfından devralınmıştır.) |
| override [SaveFormat](../../aspose.cells.lowcode/lowcodeimagesaveoptions/saveformat/) { get; set; } | Kaydetme biçimini alır veya ayarlar. |
| [SaveOptionsProvider](../../aspose.cells.lowcode/lowcodeimagesaveoptions/saveoptionsprovider/) { get; set; } | Oluşturulan görüntüleri kaydetmek için kaydetme seçenekleri sağlayıcısı. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeClassLowCodeImageSaveOptionsDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Çalışma sayfasına örnek veri ekle
                worksheet.Cells["A1"].PutValue("LowCode Image Save Demo");
                worksheet.Cells["A2"].PutValue("This demonstrates LowCodeImageSaveOptions");

                // LowCodeImageSaveOptions bir örnek oluşturun
                LowCodeImageSaveOptions saveOptions = new LowCodeImageSaveOptions();

                // Temel özellikleri ayarlayın
                saveOptions.SaveFormat = SaveFormat.Png;
                saveOptions.ImageOptions = new ImageOrPrintOptions();

                // Mevcut ayarları göster
                Console.WriteLine("SaveFormat: " + saveOptions.SaveFormat);
                Console.WriteLine("ImageOptions HorizontalResolution: " +
                    saveOptions.ImageOptions.HorizontalResolution);

                // Bazı görüntü seçeneklerini değiştir
                saveOptions.ImageOptions.HorizontalResolution = 300;
                saveOptions.ImageOptions.VerticalResolution = 300;

                // Basit bir kaydetme seçenekleri sağlayıcı oluşturun
                saveOptions.SaveOptionsProvider = new SimpleSaveOptionsProvider();

                // Çalışma sayfasını görüntü olarak kaydedin
                SheetRender renderer = new SheetRender(worksheet, saveOptions.ImageOptions);
                renderer.ToImage(0, "LowCodeImageOutput.png");

                Console.WriteLine("Image saved successfully with LowCodeImageSaveOptions");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with LowCodeImageSaveOptions: {ex.Message}");
            }
        }
    }

    public class SimpleSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            return new LowCodeImageSaveOptions()
            {
                SaveFormat = SaveFormat.Png,
                ImageOptions = new ImageOrPrintOptions()
                {
                    HorizontalResolution = 300,
                    VerticalResolution = 300
                }
            };
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            Console.WriteLine("Finished saving part");
        }
    }
}
```

### Ayrıca Bakınız

* class [LowCodeSaveOptions](../lowcodesaveoptions/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


