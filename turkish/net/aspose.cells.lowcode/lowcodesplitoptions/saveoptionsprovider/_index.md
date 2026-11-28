---
title: "LowCodeSplitOptions.SaveOptionsProvider"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LowCodeSplitOptions özelliği. Bölünmüş parçaları kaydetmek için kaydetme seçenekleri sağlayıcısı"
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodesplitoptions/saveoptionsprovider/
---
## LowCodeSplitOptions.SaveOptionsProvider property

Bölünmüş parçaları kaydetmek için kaydetme seçenekleri sağlayıcısı.

```csharp
public AbstractLowCodeSaveOptionsProvider SaveOptionsProvider { get; set; }
```

### Açıklamalar

Bu özellik belirtilirse, [`SaveOptions`](../saveoptions/) etkisiz olur çünkü her bölünmüş parçanın çıktısı sağlayıcı tarafından belirlenir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSplitOptionsPropertySaveOptionsProviderDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Biraz örnek veri doldurun
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);
            
            // LowCodeSplitOptions örneği oluştur
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            
            // Mevcut SaveOptionsProvider değerini göster (varsayılan olarak null)
            Console.WriteLine("Current SaveOptionsProvider value: " + (splitOptions.SaveOptionsProvider == null ? "null" : "not null"));
            
            // Özel bir SaveOptionsProvider oluştur
            splitOptions.SaveOptionsProvider = new CustomSaveOptionsProvider();
            
            // SaveOptionsProvider ayarlamanın etkisini göster
            // Gerçek bir senaryoda, bu dosyalar bölünürken kullanılacaktır
            Console.WriteLine("After setting SaveOptionsProvider: " + (splitOptions.SaveOptionsProvider == null ? "null" : "not null"));
            
            // Çalışma kitabını kaydet (bölünme burada gösterilmemiş olsa da)
            workbook.Save("PropertySaveOptionsProviderDemo.xlsx");
        }
    }

    // AbstractLowCodeSaveOptionsProvider'ın özel uygulaması
    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            // Her bölünmüş parça için özel kaydetme seçenekleri oluştur
            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            return options;
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            // Her parçayı kaydettikten sonra temizlik işlemlerini gerçekleştir
            Console.WriteLine("Finished saving part");
        }
    }
}
```

### Ayrıca Bakınız

* class [AbstractLowCodeSaveOptionsProvider](../../abstractlowcodesaveoptionsprovider/)
* class [LowCodeSplitOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


