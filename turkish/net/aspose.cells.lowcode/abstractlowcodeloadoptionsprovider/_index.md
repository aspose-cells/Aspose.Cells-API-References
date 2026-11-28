---
title: "Sınıf AbstractLowCodeLoadOptionsProvider"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.LowCode.AbstractLowCodeLoadOptionsProvider sınıfı. Şablon dosyaları gibi birden fazla girdi kullanan süreçler için birden çok yükleme seçeneği sağlamak amacıyla bir uygulama"
type: docs
url: /tr/net/aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/
---
## AbstractLowCodeLoadOptionsProvider class

Birden çok girdi (şablon dosyaları gibi) kullanan süreçler için birden çok yükleme seçeneği sağlamak üzere uygulanmıştır.

```csharp
public abstract class AbstractLowCodeLoadOptionsProvider
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| abstract [Current](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/current/) { get; } | Şu anda işlenen parçanın verilerini yüklemek için kullanılacak yükleme seçeneklerini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/finish/)(LowCodeLoadOptions) | Şu anda girişin işlenmiş kısmının ardından kaynakları serbest bırakır. |
| abstract [MoveNext](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/movenext/)() | Daha fazla giriş olup olmadığını kontrol eder. |

### Açıklamalar

Örneğin, [`SpreadsheetMerger`](../spreadsheetmerger/) özelliği birleştirmek için birden çok şablon dosyası gerektirir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassAbstractLowCodeLoadOptionsProviderDemo
    {
        public static void Run()
        {
            // AbstractLowCodeLoadOptionsProvider için özel bir uygulama oluşturun
            var provider = new CustomLoadOptionsProvider();

            // Sağlayıcıyı kullanarak birden çok girişi işleyin
            while (provider.MoveNext())
            {
                // Mevcut yükleme seçeneklerini alın
                LowCodeLoadOptions currentOptions = provider.Current;
                Console.WriteLine($"Processing with load options: {currentOptions}");

                // Mevcut seçeneklerle bir çalışma kitabı oluşturun
                Workbook workbook = new Workbook(FileFormatType.Xlsx);
                Worksheet worksheet = workbook.Worksheets[0];

                // Çalışma kitabı ile kullanımı gösterin
                worksheet.Cells["A1"].PutValue("Processed with custom provider");
                
                // Bu kısmın işlenmesini tamamlayın
                provider.Finish(currentOptions);
            }
        }

        private class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
        {
            private int currentIndex = 0;
            private readonly LowCodeLoadOptions[] optionsList = new LowCodeLoadOptions[]
            {
                new LowCodeLoadOptions(),
                new LowCodeLoadOptions { InputFile = "protected.xlsx" }, // Password would be handled separately
                new LowCodeLoadOptions() // MemorySetting would be handled separately
            };

            public override LowCodeLoadOptions Current => optionsList[currentIndex];

            public override bool MoveNext()
            {
                if (currentIndex < optionsList.Length - 1)
                {
                    currentIndex++;
                    return true;
                }
                return false;
            }

            public override void Finish(LowCodeLoadOptions part)
            {
                // Her bölüm için temizlik veya sonlandırma mantığı
                Console.WriteLine($"Finished processing part {currentIndex}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


