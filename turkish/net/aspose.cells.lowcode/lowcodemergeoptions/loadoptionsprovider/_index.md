---
title: "LowCodeMergeOptions.LoadOptionsProvider"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LowCodeMergeOptions özelliği. Bölünmüş parçaları kaydetmek için kaydetme seçeneklerinin sağlayıcısı"
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodemergeoptions/loadoptionsprovider/
---
## LowCodeMergeOptions.LoadOptionsProvider property

Bölünmüş parçaları kaydetmek için kaydetme seçenekleri sağlayıcısı.

```csharp
public AbstractLowCodeLoadOptionsProvider LoadOptionsProvider { get; set; }
```

### Açıklamalar

Bu özellik belirtilirse, [`LoadOptions`](../../../aspose.cells/loadoptions/) etkisiz olur çünkü her bölünmüş parçanın çıktısı sağlayıcı tarafından belirlenir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeMergeOptionsPropertyLoadOptionsProviderDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // LowCodeMergeOptions bir örnek oluştur
            LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();

            // LoadOptionsProvider'ın mevcut değerini göster (başlangıçta null olmalı)
            Console.WriteLine("Current LoadOptionsProvider value: " + (mergeOptions.LoadOptionsProvider == null ? "null" : "not null"));

            // Özel bir LoadOptionsProvider uygulaması oluştur
            mergeOptions.LoadOptionsProvider = new CustomLoadOptionsProvider();

            // Özelliği ayarlamayı göster
            Console.WriteLine("After setting LoadOptionsProvider: " + (mergeOptions.LoadOptionsProvider == null ? "null" : "not null"));

            // Birleştirme seçeneklerini sağlayıcıyla kullan
            // Bu genellikle birden çok dosyayı işleyen yöntemlerle kullanılır
            // Gösterim amacıyla, sağlayıcının bir sonraki adıma geçip geçemeyeceğini kontrol edeceğiz
            bool hasNext = mergeOptions.LoadOptionsProvider.MoveNext();
            Console.WriteLine("LoadOptionsProvider MoveNext result: " + hasNext);

            // Çalışma kitabını kaydedin
            workbook.Save("PropertyLoadOptionsProviderDemo.xlsx");
        }

        private class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
        {
            private int counter = 0;
            private readonly LowCodeLoadOptions options = new LowCodeLoadOptions();

            public override LowCodeLoadOptions Current => options;

            public override bool MoveNext()
            {
                // İşlenecek 3 dosya olduğunu taklit et
                if (counter < 3)
                {
                    counter++;
                    return true;
                }
                return false;
            }

            public override void Finish(LowCodeLoadOptions part)
            {
                // Temizleme veya sonlandırma mantığı burada olur
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [AbstractLowCodeLoadOptionsProvider](../../abstractlowcodeloadoptionsprovider/)
* class [LowCodeMergeOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


