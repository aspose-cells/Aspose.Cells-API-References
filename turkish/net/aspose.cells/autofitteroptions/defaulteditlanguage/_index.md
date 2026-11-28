---
title: "AutoFitterOptions.DefaultEditLanguage"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AutoFitterOptions özelliği. Varsayılan düzenleme dilini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/autofitteroptions/defaulteditlanguage/
---
## AutoFitterOptions.DefaultEditLanguage property

Varsayılan düzenleme dilini alır veya ayarlar.

```csharp
public DefaultEditLanguage DefaultEditLanguage { get; set; }
```

### Açıklamalar

Farklı düzenleme dilleri ayarlandığında metin paragrafı için farklı düzenler görüntülenebilir/işlenebilir. Varsayılan değer Auto'dur.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyDefaultEditLanguageDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir hücreye örnek CJK metni ayarlayın
            worksheet.Cells["A1"].PutValue("日本語のテキスト");

            AutoFitterOptions options = new AutoFitterOptions();
            options.DefaultEditLanguage = DefaultEditLanguage.CJK;

            // CJK dil ayarlarıyla satırı otomatik olarak ayarlayın
            worksheet.AutoFitRows(options);

            Console.WriteLine("Auto-fit completed with DefaultEditLanguage: " + options.DefaultEditLanguage);
            workbook.Save("DefaultEditLanguageDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [DefaultEditLanguage](../../defaulteditlanguage/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


