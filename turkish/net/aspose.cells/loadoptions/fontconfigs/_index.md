---
title: "LoadOptions.FontConfigs"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LoadOptions özelliği. Tek tek yazı tipi yapılandırmalarını alır ve ayarlar. Yalnızca bu LoadOptions'ı kullanarak yükleyen Workbook için çalışır"
type: docs
url: /tr/net/aspose.cells/loadoptions/fontconfigs/
---
## LoadOptions.FontConfigs property

Tek tek yazı tipi yapılandırmalarını alır ve ayarlar. Yalnızca [`Workbook`](../../workbook/) bu [`LoadOptions`](../) ile yüklendiğinde çalışır.

```csharp
public IndividualFontConfigs FontConfigs { get; set; }
```

### Örnekler

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyFontConfigsDemo
    {
        public static void Run()
        {
            // FontConfigs ile yükleme seçenekleri oluşturun
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                FontConfigs = new IndividualFontConfigs()
            };

            // Doğru API'yi kullanarak bazı yazı tipi ikame kuralları ayarlayın
            loadOptions.FontConfigs.SetFontSubstitutes("Arial", new string[] { "Times New Roman" });
            loadOptions.FontConfigs.SetFontSubstitutes("Courier New", new string[] { "Consolas" });

            // Belirtilen seçeneklerle bir CSV dosyası yükleyin
            Workbook workbook = new Workbook("sample.csv", loadOptions);

            // Çalışma kitabını bir Excel dosyasına kaydet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [IndividualFontConfigs](../../individualfontconfigs/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


