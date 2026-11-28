---
title: "HtmlSaveOptions.DefaultFontName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Html dışa aktarımı için varsayılan yazı tipi adını belirtir; stilin yazı tipi mevcut değilse varsayılan yazı tipi kullanılır. Bu özellik null ise Aspose.Cells, orijinal yazı tipiyle aynı aileye sahip evrensel bir yazı tipi kullanır. Varsayılan değer null'dur."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/defaultfontname/
---
## HtmlSaveOptions.DefaultFontName property

HTML dışa aktarımı için varsayılan yazı tipi adını belirtin, stilin yazı tipi mevcut değilse varsayılan yazı tipi kullanılacaktır. Bu özellik null ise, Aspose.Cells aynı aileye sahip evrensel bir yazı tipi kullanır, varsayılan değer null'dur.

```csharp
public string DefaultFontName { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyDefaultFontNameDemo
    {
        public static void Run()
        {
            // Örnek bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Sample Text");
            
            // Özel varsayılan yazı tipiyle HTML kaydetme seçeneklerini ayarlayın
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.DefaultFontName = "Courier New";
            
            // Belirtilen yazı tipiyle HTML'ye kaydedin
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML file saved with default font: " + saveOptions.DefaultFontName);
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


