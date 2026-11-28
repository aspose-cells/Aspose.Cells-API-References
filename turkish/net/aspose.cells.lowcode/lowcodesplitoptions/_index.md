---
title: "LowCodeSplitOptions sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.LowCode.LowCodeSplitOptions sınıfı. Elektronik tabloyu bölmek için seçenekler"
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodesplitoptions/
---
## LowCodeSplitOptions class

Elektronik tabloyu bölme seçenekleri.

```csharp
public class LowCodeSplitOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [LowCodeSplitOptions](lowcodesplitoptions/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [LoadOptions](../../aspose.cells.lowcode/lowcodesplitoptions/loadoptions/) { get; set; } | Bölünecek elektronik tabloyu yüklemek için yükleme seçenekleri. |
| [SaveOptions](../../aspose.cells.lowcode/lowcodesplitoptions/saveoptions/) { get; set; } | Bölünmüş parçaları kaydetmek için kaydetme seçenekleri. |
| [SaveOptionsProvider](../../aspose.cells.lowcode/lowcodesplitoptions/saveoptionsprovider/) { get; set; } | Bölünmüş parçaları kaydetmek için kaydetme seçenekleri sağlayıcısı. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassLowCodeSplitOptionsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasını örnek verilerle doldurun
            worksheet.Cells["A1"].PutValue("Sample Data for Splitting");
            
            // LowCodeSplitOptions sınıfının bir örneğini oluşturun
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            
            // LoadOptions'ı yapılandırın (örnek: şifre korumalı kaynağı işleyin)
            splitOptions.LoadOptions = new LowCodeLoadOptions();
            
            // SaveOptions'ı yapılandırın (örnek: varsayılan çıktı formatını ayarlayın)
            splitOptions.SaveOptions = new LowCodeSaveOptions();
            
            // Dinamik çıktı ayarları için özel SaveOptions sağlayıcısını uygulayın
            splitOptions.SaveOptionsProvider = new CustomSaveOptionsProvider();
            
            // Örnek entegrasyon: Çalışma kitabını yapılandırılmış seçeneklerle parçalara bölün
            // (LowCodeEngine.Split(workbook, splitOptions, "outputDir") gibi bir yöntemin var olduğunu varsayın)
            // LowCodeEngine.Split(workbook, splitOptions, "OutputDirectory");
            
            // Demonstrasyon için orijinal çalışma kitabını kaydedin
            workbook.Save("LowCodeSplitOptionsDemo.xlsx");
        }

        // Özel SaveOptionsProvider uygulaması
        private class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
        {
            public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
            {
                // Örnek mantık: Bölme indeksine göre ayarları değiştirin
                return new LowCodeSaveOptions();
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


