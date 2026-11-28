---
title: "PageSetup.PrinterSettings"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Varsayılan yazıcının ayarlarını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/pagesetup/printersettings/
---
## PageSetup.PrinterSettings property

Varsayılan yazıcının ayarlarını alır ve ayarlar.

```csharp
public byte[] PrinterSettings { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrinterSettingsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına bazı veriler ekle
            worksheet.Cells["A1"].PutValue("Test Printer Settings");
            
            // Sayfa ayarına eriş
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Yazıcı ayarlarını (bayt dizisi olarak) ayarlayın
            byte[] printerSettings = new byte[10]; // Simplified example
            pageSetup.PrinterSettings = printerSettings;
            
            // Yazıcı ayarlarının ayarlandığını doğrulayın
            Console.WriteLine("Printer Settings: " + (pageSetup.PrinterSettings != null));
            
            // Çalışma kitabını kaydedin
            workbook.Save("PrinterSettingsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


