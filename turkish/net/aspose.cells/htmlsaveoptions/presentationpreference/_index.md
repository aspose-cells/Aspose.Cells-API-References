---
title: "HtmlSaveOptions.PresentationPreference"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. HTML veya MHT dosyasının sunum tercihi olup olmadığını gösterir. Varsayılan değer false'tur. Daha güzel bir sunum elde etmek istiyorsanız değeri true olarak ayarlayın."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/presentationpreference/
---
## HtmlSaveOptions.PresentationPreference property

Html veya mht dosyasının sunum tercihi olup olmadığını gösterir. Varsayılan değer false'tur. Daha güzel bir sunum elde etmek istiyorsanız, değeri true olarak ayarlayın.

```csharp
public bool PresentationPreference { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyPresentationPreferenceDemo
    {
        public static void Run()
        {
            // Test verileriyle örnek bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Presentation Preference Test");
            worksheet.Cells["B1"].PutValue(123.45);
            worksheet.Cells["A2"].PutValue(DateTime.Now);

            // PresentationPreference ile HTML kaydetme seçeneklerini ayarlayın
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.PresentationPreference = true;
            options.IsFullPathLink = false;

            // Demonstrasyon için bellek akışına kaydedin
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, options);
                Console.WriteLine("Workbook saved with PresentationPreference=true");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


