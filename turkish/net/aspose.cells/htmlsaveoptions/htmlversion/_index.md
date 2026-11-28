---
title: "HtmlSaveOptions.HtmlVersion"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. HTML formatı kaydedilirken kullanılacak HTML standardının sürümünü belirtir. Varsayılan değer HtmlVersion.Default'tir."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/htmlversion/
---
## HtmlSaveOptions.HtmlVersion property

HTML standardının hangi sürümünün HTML formatı kaydedilirken kullanılacağını belirtir. Varsayılan değer "HtmlVersion.Default"'tır.

```csharp
public HtmlVersion HtmlVersion { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlSaveOptionsPropertyHtmlVersionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("HTML Version Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates HtmlVersion property");
            worksheet.Cells["B3"].PutValue(123.45);
            worksheet.Cells["C4"].PutValue("Sample Text");
            
            // HtmlSaveOptions örneği oluştur
            HtmlSaveOptions options = new HtmlSaveOptions();
            
            // Mevcut HtmlVersion değerini göster
            Console.WriteLine("Current HtmlVersion: " + options.HtmlVersion);
            
            // HtmlVersion'ı HTML5 olarak ayarla
            options.HtmlVersion = HtmlVersion.Html5;
            Console.WriteLine("HtmlVersion changed to: " + options.HtmlVersion);
            
            // HTML5 sürümüyle kaydet
            workbook.Save("HtmlVersion_Html5.html", options);
            
            // XHTML'ye değiştir
            options.HtmlVersion = HtmlVersion.XHtml;
            Console.WriteLine("HtmlVersion changed to: " + options.HtmlVersion);
            
            // XHTML sürümüyle kaydet
            workbook.Save("HtmlVersion_XHtml.html", options);
            
            // Varsayılan ayarlara sıfırla
            options.HtmlVersion = HtmlVersion.Default;
            Console.WriteLine("HtmlVersion reset to: " + options.HtmlVersion);
            
            // Varsayılan sürümle kaydet
            workbook.Save("HtmlVersion_Default.html", options);
        }
    }
}
```

### Ayrıca Bakınız

* enum [HtmlVersion](../../htmlversion/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


