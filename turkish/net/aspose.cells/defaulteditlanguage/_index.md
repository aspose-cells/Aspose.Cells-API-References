---
title: "Enum DefaultEditLanguage"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.DefaultEditLanguage enum. Varsayılan düzenleme dilini temsil eder"
type: docs
url: /tr/net/aspose.cells/defaulteditlanguage/
---
## DefaultEditLanguage enumeration

Varsayılan düzenleme dilini temsil eder.

```csharp
public enum DefaultEditLanguage
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Auto | `0` | Metne göre otomatik olarak düzenleme dilini algılamayı temsil eder. |
| English | `1` | İngilizce dilini temsil eder. |
| CJK | `2` | Çince, Japonca ve Korece dilleri temsil eder. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DefaultEditLanguageDemo
    {
        public static void DefaultEditLanguageExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // AutoFitterOptions oluşturun ve DefaultEditLanguage ayarlayın
            AutoFitterOptions autoFitterOptions = new AutoFitterOptions();
            autoFitterOptions.DefaultEditLanguage = DefaultEditLanguage.CJK;

            // Belirtilen seçeneklerle otomatik satır sığdırmayı uygulayın
            worksheet.AutoFitRows(autoFitterOptions);

            // Çalışma kitabını kaydedin
            workbook.Save("DefaultEditLanguageExample.xlsx");
            workbook.Save("DefaultEditLanguageExample.pdf");

            // Ayarlanan DefaultEditLanguage'i konsola çıktılayın
            Console.WriteLine("Default Edit Language set to: " + autoFitterOptions.DefaultEditLanguage);
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


