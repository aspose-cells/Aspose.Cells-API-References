---
title: "Sınıf LowCodeMergeOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.LowCode.LowCodeMergeOptions sınıfı. Birden fazla şablon dosyasını tek bir dosyada birleştirme seçenekleri"
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodemergeoptions/
---
## LowCodeMergeOptions class

Birden çok şablon dosyasını tek bir dosyada birleştirme seçenekleri.

```csharp
public class LowCodeMergeOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [LowCodeMergeOptions](lowcodemergeoptions/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [LoadOptionsProvider](../../aspose.cells.lowcode/lowcodemergeoptions/loadoptionsprovider/) { get; set; } | Bölünmüş parçaları kaydetmek için kaydetme seçenekleri sağlayıcısı. |
| [SaveOptions](../../aspose.cells.lowcode/lowcodemergeoptions/saveoptions/) { get; set; } | Bölünmüş parçaları kaydetmek için kaydetme seçenekleri. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassLowCodeMergeOptionsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // LowCodeMergeOptions oluşturun ve yapılandırın
            LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();
            
            // Çıktı formatı için kaydetme seçeneklerini ayarlayın
            mergeOptions.SaveOptions = new LowCodeSaveOptions();
            
            // Özel yükleme seçenekleri sağlayıcısını atayın
            mergeOptions.LoadOptionsProvider = new CustomLoadOptionsProvider();
            
            // Örnek entegrasyon (birleştirme işlevselliğiyle varsayımsal kullanım)
            // Bu genellikle gerçek dosya yolları ile çağrılır
            // Workbook.Merge(new string[] { "template1.xlsx", "template2.xlsx" }, mergeOptions);
            
            // Çalışma kitabını kaydedin (gösterim amaçlarıyla)
            workbook.Save("LowCodeMergeOptionsDemo.xlsx");
        }
    }

    // Soyut sınıfı uygulayan özel sağlayıcı
    public class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
    {
        public override bool MoveNext()
        {
            // Soyut gereksinimi karşılamak için minimal uygulama
            return false;
        }

        public override LowCodeLoadOptions Current
        {
            get { throw new InvalidOperationException(); }
        }

        public LoadOptions GetLoadOptions(string fileName)
        {
            if (fileName.EndsWith(".xlsx", StringComparison.OrdinalIgnoreCase))
            {
                return new LoadOptions(LoadFormat.Xlsx);
            }
            return new LoadOptions();
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


