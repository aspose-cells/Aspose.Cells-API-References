---
title: "WorkbookSettings.LanguageCode"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Dosyanın kaydedildiği CountryCode'a göre Çalışma Kitabı sürümünün kullanıcı arayüzü dilini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/workbooksettings/languagecode/
---
## WorkbookSettings.LanguageCode property

Dosyayı kaydeden CountryCode temelinde Workbook sürümünün kullanıcı arayüzü dilini alır veya ayarlar.

```csharp
public CountryCode LanguageCode { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyLanguageCodeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabı ayarlarına eriş
            WorkbookSettings settings = workbook.Settings;

            // Dil kodunu Almanca (Almanya) olarak ayarla
            settings.LanguageCode = CountryCode.Germany;

            // Mevcut dil kodunu göster
            Console.WriteLine("Current Language Code: " + settings.LanguageCode);

            // Dil kodunu Fransızca (Fransa) olarak değiştir
            settings.LanguageCode = CountryCode.France;
            Console.WriteLine("Updated Language Code: " + settings.LanguageCode);

            // Çalışma kitabını kaydedin
            workbook.Save("WorkbookSettings_LanguageCodeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [CountryCode](../../countrycode/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


