---
title: "HtmlSaveOptions.IsFullPathLink"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. sheet00x.htmfilelist.xml ve tabstrip.htm içinde tam yol bağlantısı kullanılıp kullanılmadığını gösterir. Varsayılan değer false'tur."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/isfullpathlink/
---
## HtmlSaveOptions.IsFullPathLink property

sheet00x.htm, filelist.xml ve tabstrip.htm içinde tam yol bağlantısı kullanılıp kullanılmayacağını gösterir. Varsayılan değer false'tur.

```csharp
public bool IsFullPathLink { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsFullPathLinkDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test HTML Export");

            // HTML kaydetme seçenekleri oluştur
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // IsFullPathLink özelliğini göster
            saveOptions.IsFullPathLink = true; // Set to true to use full path links
            
            // Farklı IsFullPathLink ayarlarıyla kaydet
            workbook.Save("HtmlExport_FullPathLinks.html", saveOptions);
            
            saveOptions.IsFullPathLink = false; // Set to false for relative paths
            workbook.Save("HtmlExport_RelativeLinks.html", saveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


