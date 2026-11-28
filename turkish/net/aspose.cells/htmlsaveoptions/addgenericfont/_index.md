---
title: "HtmlSaveOptions.AddGenericFont"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. CSS fontfamily'ye genel bir yazı tipi eklenip eklenmeyeceğini gösterir. Varsayılan değer true'tur"
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/addgenericfont/
---
## HtmlSaveOptions.AddGenericFont property

CSS font-family'ye genel bir yazı tipinin eklenip eklenmeyeceğini gösterir. Varsayılan değer true'tur.

```csharp
public bool AddGenericFont { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyAddGenericFontDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Belirli bir yazı tipiyle örnek metni ayarla
            var cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");
            Style style = cell.GetStyle();
            style.Font.Name = "Pacifico";
            cell.SetStyle(style);

            // AddGenericFont etkin (varsayılan) ile kaydet
            HtmlSaveOptions options = new HtmlSaveOptions(SaveFormat.Html);
            workbook.Save("output_with_generic.html", options);

            // AddGenericFont devre dışı bırakılmış şekilde kaydet
            options.AddGenericFont = false;
            workbook.Save("output_without_generic.html", options);

            // Sonuçları doğrulayın
            string withGeneric = File.ReadAllText("output_with_generic.html");
            string withoutGeneric = File.ReadAllText("output_without_generic.html");

            Console.WriteLine("With generic font: " + (withGeneric.Contains("font-family:Pacifico,sans-serif") ? "Found" : "Not found"));
            Console.WriteLine("Without generic font: " + (withoutGeneric.Contains("font-family:Pacifico,sans-serif") ? "Found" : "Not found"));
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


