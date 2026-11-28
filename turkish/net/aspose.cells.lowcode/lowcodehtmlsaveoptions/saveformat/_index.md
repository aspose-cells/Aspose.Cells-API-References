---
title: "LowCodeHtmlSaveOptions.SaveFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LowCodeHtmlSaveOptions özelliği. Elektronik tablo formatını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodehtmlsaveoptions/saveformat/
---
## LowCodeHtmlSaveOptions.SaveFormat property

Çalışma sayfasının formatını alır ve ayarlar.

```csharp
public override SaveFormat SaveFormat { get; set; }
```

### Açıklamalar

Bu özellik değiştirildiğinde, [`HtmlOptions`](../htmloptions/) tarafından belirtilen kaydetme formatı yok sayılacak (daha önce belirtilmişse).

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeHtmlSaveOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample HTML Export");

            LowCodeHtmlSaveOptions options = new LowCodeHtmlSaveOptions();
            Console.WriteLine("Current SaveFormat value: " + options.SaveFormat);

            options.SaveFormat = SaveFormat.Html;
            options.HtmlOptions = new HtmlSaveOptions();

            workbook.Save("LowCodeHtmlExport.html", options.HtmlOptions);
        }
    }
}
```

### Ayrıca Bakınız

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodeHtmlSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


