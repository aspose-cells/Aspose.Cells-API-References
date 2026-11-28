---
title: "LowCodeImageSaveOptions.SaveOptionsProvider"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LowCodeImageSaveOptions özelliği. Oluşturulan görüntüleri kaydetmek için kaydetme seçeneklerinin sağlayıcısı"
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodeimagesaveoptions/saveoptionsprovider/
---
## LowCodeImageSaveOptions.SaveOptionsProvider property

Oluşturulan görüntüleri kaydetmek için kaydetme seçenekleri sağlayıcısı.

```csharp
public AbstractLowCodeSaveOptionsProvider SaveOptionsProvider { get; set; }
```

### Açıklamalar

Bu örnek tarafından belirtilen çıktı([`OutputFile`](../../lowcodesaveoptions/outputfile/) veya [`OutputStream`](../../lowcodesaveoptions/outputstream/)) bu özellik belirtildiğinde etkili olmayacaktır. Bunun yerine her oluşturulan görüntünün çıktısı sağlayıcı tarafından belirlenecektir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeImageSaveOptionsPropertySaveOptionsProviderDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Sample Image Data");
            
            // LowCodeImageSaveOptions örneği oluşturun
            LowCodeImageSaveOptions saveOptions = new LowCodeImageSaveOptions();
            saveOptions.SaveFormat = SaveFormat.Png;
            saveOptions.ImageOptions = new ImageOrPrintOptions();
            
            // Özel bir SaveOptionsProvider oluştur
            CustomSaveOptionsProvider provider = new CustomSaveOptionsProvider();
            saveOptions.SaveOptionsProvider = provider;
            
            // Mevcut SaveOptionsProvider'ı göster
            Console.WriteLine("Current SaveOptionsProvider: " + (saveOptions.SaveOptionsProvider != null ? "Custom Provider" : "null"));
            
            // Farklı seçeneklerle kaydederek etkiyi göster
            workbook.Save("output_with_provider.png", saveOptions.SaveFormat);
            
            // Sağlayıcıyı null olarak değiştir
            saveOptions.SaveOptionsProvider = null;
            Console.WriteLine("Changed SaveOptionsProvider to: " + (saveOptions.SaveOptionsProvider != null ? "Custom Provider" : "null"));
            
            workbook.Save("output_without_provider.png", saveOptions.SaveFormat);
        }
    }

    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            // Her bölüm için özel kaydetme seçeneklerini döndür
            return new LowCodeImageSaveOptions()
            {
                SaveFormat = SaveFormat.Jpg,  // Changed from Jpeg to Jpg
                ImageOptions = new ImageOrPrintOptions()
                {
                    Quality = 90,
                    HorizontalResolution = 300,
                    VerticalResolution = 300
                }
            };
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            // Kaydettikten sonra gerekli temizlik işlemlerini yap
            Console.WriteLine("Finished saving part with custom options");
        }
    }
}
```

### Ayrıca Bakınız

* class [AbstractLowCodeSaveOptionsProvider](../../abstractlowcodesaveoptionsprovider/)
* class [LowCodeImageSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


