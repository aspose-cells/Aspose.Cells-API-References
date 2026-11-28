---
title: "HtmlLoadOptions.ProgId"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlLoadOptions özelliği. Dosyayı oluşturmanın program kimliğini alır. Yalnızca MHT dosyaları için"
type: docs
url: /tr/net/aspose.cells/htmlloadoptions/progid/
---
## HtmlLoadOptions.ProgId property

Dosyanın oluşturulması için program kimliğini alır. Yalnızca MHT dosyaları için.

```csharp
public string ProgId { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyProgIdDemo
    {
        public static void Run()
        {
            // MHTML formatı ile HTML yükleme seçenekleri oluştur
            HtmlLoadOptions options = new HtmlLoadOptions(LoadFormat.MHtml);
            
            // ProgId özelliğini al
            Console.WriteLine("ProgId is: " + options.ProgId);

            // Başka bir örnek oluştur ve onun ProgId'sini al
            HtmlLoadOptions wordOptions = new HtmlLoadOptions(LoadFormat.MHtml);
            Console.WriteLine("ProgId is: " + wordOptions.ProgId);
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


