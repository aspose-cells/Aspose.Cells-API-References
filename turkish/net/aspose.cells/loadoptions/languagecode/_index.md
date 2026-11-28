---
title: "LoadOptions.LanguageCode"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LoadOptions özelliği. Dosyayı kaydeden CountryCode'a göre Workbook sürümünün kullanıcı arayüzü dilini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/loadoptions/languagecode/
---
## LoadOptions.LanguageCode property

Dosyayı kaydeden CountryCode temelinde Workbook sürümünün kullanıcı arayüzü dilini alır veya ayarlar.

```csharp
public CountryCode LanguageCode { get; set; }
```

### Örnekler

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyLanguageCodeDemo
    {
        public static void Run()
        {
            // LoadOptions bir örnek oluşturur.
            LoadOptions loadOptions = new LoadOptions();

            // LanguageCode özelliğini ayarla
            loadOptions.LanguageCode = CountryCode.USA;

            // Belirtilen LoadOptions ile bir çalışma kitabı yükleyin
            Workbook workbook = new Workbook("sample.xlsx", loadOptions);

            // Çalışma sayfasına eriş ve içeriği değiştir
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Language Code Demo");

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [CountryCode](../../countrycode/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


