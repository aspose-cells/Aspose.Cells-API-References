---
title: "LowCodeSplitOptions.LoadOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LowCodeSplitOptions özelliği. Bölünecek elektronik tabloyu yüklemek için yükleme seçenekleri"
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodesplitoptions/loadoptions/
---
## LowCodeSplitOptions.LoadOptions property

Bölünecek elektronik tabloyu yüklemek için yükleme seçenekleri.

```csharp
public LowCodeLoadOptions LoadOptions { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSplitOptionsPropertyLoadOptionsDemo
    {
        public static void Run()
        {
            // Bölme seçenekleri örneği oluşturun
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();

            // Yükleme seçeneklerini başlat
            splitOptions.LoadOptions = new LowCodeLoadOptions();

            // Farklı ayarlarla yeni yükleme seçenekleri oluşturun (mevcut özellikleri kullanarak)
            splitOptions.LoadOptions = new LowCodeLoadOptions();
            
            // Son yapılandırmayı gösterin
            Console.WriteLine("LoadOptions configured with InputFile: " + splitOptions.LoadOptions.InputFile);
        }
    }
}
```

### Ayrıca Bakınız

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSplitOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


