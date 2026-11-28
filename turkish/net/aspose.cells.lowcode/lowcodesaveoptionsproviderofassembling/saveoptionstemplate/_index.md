---
title: "LowCodeSaveOptionsProviderOfAssembling.SaveOptionsTemplate"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LowCodeSaveOptionsProviderOfAssembling özelliği. GetSaveOptions içinde kaydetme seçenekleri örneği oluşturmak için şablon"
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/saveoptionstemplate/
---
## LowCodeSaveOptionsProviderOfAssembling.SaveOptionsTemplate property

Kaydetme seçenekleri örneği oluşturmak için [`GetSaveOptions`](../getsaveoptions/) içinde şablon.

```csharp
public LowCodeSaveOptions SaveOptionsTemplate { get; set; }
```

### Açıklamalar

Şablon belirtilmişse, oluşturulan örnek tüm ayarları ondan kopyalar ve çıktı dosyasını buna göre günceller.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Saving;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertySaveOptionsTemplateDemo
    {
        public static void Run()
        {
            // İki çalışma sayfası içeren yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            Worksheet worksheet1 = workbook.Worksheets[0];
            Worksheet worksheet2 = workbook.Worksheets[1];
            worksheet1.Cells["A1"].PutValue("Sheet1 Content");
            worksheet2.Cells["A1"].PutValue("Sheet2 Content");

            // LowCodeSaveOptionsProviderOfAssembling örneği oluştur
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "Output/Sheet",
                PathTail = ".xlsx",
                BuildPathWithSheetAlways = true,
                UseSheetName = false
            };

            // İlk SaveOptionsTemplate durumunu göster
            Console.WriteLine("Initial SaveOptionsTemplate is " + (provider.SaveOptionsTemplate == null ? "null" : "set"));

            // SaveOptionsTemplate'i şifreleme ile yapılandır
            provider.SaveOptionsTemplate = new LowCodeSaveOptions();
            Console.WriteLine("SaveOptionsTemplate configured");

            // LowCode kaydetme seçeneklerini oluştur
            var saveOptions = new LowCodeSaveOptions();

            // Yapılandırılmış sağlayıcıyı kullanarak çalışma kitabını kaydet (her sayfa için ayrı dosyalar oluşturur)
            workbook.Save("output_combined.xlsx", saveOptions.SaveFormat);

            Console.WriteLine("Demo executed successfully. Check output files.");
        }
    }
}
```

### Ayrıca Bakınız

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


