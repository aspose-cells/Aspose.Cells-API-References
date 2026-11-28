---
title: "HtmlSaveOptions.LinkTargetType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Bir bağlantıda hedef özniteliğinin tipini gösterir. Varsayılan değer HtmlLinkTargetType.Parent'tır."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/linktargettype/
---
## HtmlSaveOptions.LinkTargetType property

`<a>` bağlantısındaki target özniteliğinin tipini gösterir. Varsayılan değer HtmlLinkTargetType.Parent'dır.

```csharp
public HtmlLinkTargetType LinkTargetType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyLinkTargetTypeDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Link to Google");
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.google.com");

            // LinkTargetType ile HTML kaydetme seçeneklerini ayarlayın
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.LinkTargetType = HtmlLinkTargetType.Blank;

            // Çalışma kitabını HTML olarak kaydet
            workbook.Save("output.html", saveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* enum [HtmlLinkTargetType](../../htmllinktargettype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


