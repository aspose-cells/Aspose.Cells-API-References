---
title: "HtmlSaveOptions.DisableCss"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. CSS'ye dayanılmadan yalnızca satır içi stillerin uygulanıp uygulanmayacağını gösterir. Varsayılan değer false."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/disablecss/
---
## HtmlSaveOptions.DisableCss property

Yalnızca satır içi stillerin uygulanıp uygulanmayacağını, CSS'ye dayanılmadan gösterir. Varsayılan değer false'tur.

```csharp
public bool DisableCss { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlSaveOptionsPropertyDisableCssDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ve biçimlendirme ekleyin.
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A1"].GetStyle().Font.IsBold = true;
            worksheet.Cells["A1"].GetStyle().Font.Color = System.Drawing.Color.Red;
            worksheet.Cells["B1"].PutValue("Formatted Cell");
            worksheet.Cells["B1"].GetStyle().Font.IsItalic = true;
            worksheet.Cells["B1"].GetStyle().Font.Underline = FontUnderlineType.Single;

            // HtmlSaveOptions örneği oluştur
            HtmlSaveOptions options = new HtmlSaveOptions();

            // Mevcut DisableCss değerini gösterin.
            Console.WriteLine("Current DisableCss value: " + options.DisableCss);

            // DisableCss'i true olarak ayarlayın (CSS yerine satır içi stiller kullanarak).
            options.DisableCss = true;
            workbook.Save("HtmlWithInlineStyles.html", options);

            // DisableCss'i false olarak ayarlayın (CSS stilleri kullanarak).
            options.DisableCss = false;
            workbook.Save("HtmlWithCssStyles.html", options);

            // Stil yaklaşımındaki farkı görmek için çıktı dosyalarını karşılaştırın.
            Console.WriteLine("Files saved with different DisableCss settings.");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


