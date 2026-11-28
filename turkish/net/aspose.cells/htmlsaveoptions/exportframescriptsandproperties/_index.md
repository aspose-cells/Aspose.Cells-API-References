---
title: "HtmlSaveOptions.ExportFrameScriptsAndProperties"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Çerçeve betiklerinin ve belge özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'tır. HTML veya MHT dosyasını Excel'e içe aktarmak istiyorsanız lütfen varsayılan değeri koruyun."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/exportframescriptsandproperties/
---
## HtmlSaveOptions.ExportFrameScriptsAndProperties property

Çerçeve betiklerinin ve belge özelliklerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'dur. HTML veya MHT dosyasını Excel'e içe aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.

```csharp
public bool ExportFrameScriptsAndProperties { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportFrameScriptsAndPropertiesDemo
    {
        public static void Run()
        {
            // Örnek bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // ExportFrameScriptsAndProperties ile HTML kaydetme seçeneklerini ayarla
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportFrameScriptsAndProperties = true;

            // HTML olarak kaydet
            workbook.Save("output.html", options);

            Console.WriteLine("HTML file saved with ExportFrameScriptsAndProperties enabled.");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


