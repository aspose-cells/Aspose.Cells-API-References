---
title: "LoadOptions.MemorySetting"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LoadOptions özelliği. Yüklenen çalışma kitabı için bellek modunu alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/loadoptions/memorysetting/
---
## LoadOptions.MemorySetting property

Yüklenen çalışma kitabı için bellek modunu alır veya ayarlar.

```csharp
public MemorySetting MemorySetting { get; set; }
```

### Açıklamalar

Bellek modu hakkında daha fazla ayrıntı için lütfen [`MemorySetting`](../../cells/memorysetting/) adresine bakın.

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyMemorySettingDemo
    {
        public static void Run()
        {
            // Bellek tercihi ayarıyla yükleme seçenekleri oluşturun
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Auto);
            loadOptions.MemorySetting = MemorySetting.MemoryPreference;

            // Bellek optimize edilmiş ayarlarla çalışma kitabını yükleyin
            Workbook workbook = new Workbook(new MemoryStream(), loadOptions);
            
            // Çalışma sayfasına eriş ve bazı örnek veriler ekle
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Memory Setting Demo");
            worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());
            
            // Çalışma kitabını kaydedin
            workbook.Save("MemorySettingDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with MemoryPreference setting.");
        }
    }
}
```

### Ayrıca Bakınız

* enum [MemorySetting](../../memorysetting/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


