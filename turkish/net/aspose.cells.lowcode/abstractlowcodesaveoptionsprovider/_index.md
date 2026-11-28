---
title: "Sınıf AbstractLowCodeSaveOptionsProvider"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.LowCode.AbstractLowCodeSaveOptionsProvider sınıfı. Birden fazla çıktı gerektiren işlemler için birden çok kaydetme seçeneği sağlayan uygulama. Örneğin SpreadsheetSplitter özelliği, bölünmüş dosyaları kaydetmek için birden çok hedef gerektirir"
type: docs
url: /tr/net/aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/
---
## AbstractLowCodeSaveOptionsProvider class

Birden fazla çıktı gerektiren işlemler için birden çok kaydetme seçeneği sağlayan uygulama. Örneğin, [`SpreadsheetSplitter`](../spreadsheetsplitter/) özelliği, bölünmüş dosyaları kaydetmek için birden çok hedef gerektirir.

```csharp
public abstract class AbstractLowCodeSaveOptionsProvider
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/)(LowCodeSaveOptions) | Şu anda bölünmüş parçayı işledikten sonra kaynakları serbest bırakır. |
| abstract [GetSaveOptions](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/getsaveoptions/)(SplitPartInfo) | Şu anda bölünmüş parça için çıktı ayarlarını almak üzere kaydetme seçeneklerini alır. Null döndürmek, verilen parçayı atlamak anlamına gelir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassAbstractLowCodeSaveOptionsProviderDemo
    {
        public static void Run()
        {
            // AbstractLowCodeSaveOptionsProvider sınıfını genişleterek özel bir sağlayıcı oluşturun
            var customProvider = new CustomSaveOptionsProvider();

            // Bir çalışma kitabı ve çalışma sayfası oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bazı verileri doldurun
            worksheet.Cells["A1"].PutValue("Test Data");
            
            // Bölünmüş parça bilgisi oluşturun - gerçek kullanımda, bu API'den gelir
            // Doğrudan oluşturamadığımız için, gösterim amacıyla sadece null geçeceğiz
            SplitPartInfo splitPartInfo = null;
            
            // Sağlayıcıdan kaydetme seçeneklerini alın
            LowCodeSaveOptions saveOptions = customProvider.GetSaveOptions(splitPartInfo);
            
            // Kaydetme seçeneklerini yapılandırın (örnek)
            saveOptions.SaveFormat = SaveFormat.Xlsx;
            
            // İşlemi tamamlamayı gösterin
            customProvider.Finish(saveOptions);
            
            // Çalışma kitabını kaydedin (sağlayıcıyla doğrudan ilgili değil, sadece demo amaçlı)
            workbook.Save("LowCodeSaveOptionsDemo.xlsx");
        }
    }

    // AbstractLowCodeSaveOptionsProvider'ın özel uygulaması
    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            // Parça bilgisine dayanarak özel kaydetme seçenekleri oluşturun ve döndürün
            return new LowCodeSaveOptions()
            {
                SaveFormat = SaveFormat.Xlsx
                // LowCodeSaveOptions içinde bulunmadığı için CachedFileFolder kaldırıldı
            };
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            // Burada temizlik veya sonlandırma mantığını ekleyin
            Console.WriteLine("Save operation completed for part");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


