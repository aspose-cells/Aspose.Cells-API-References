---
title: "HtmlSaveOptions.ParseHtmlTagInCell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Hücredeki div/div gibi HTML etiketlerinin hücre değeri olarak ayrıştırılıp ayrıştırılmayacağını veya olduğu gibi korunacağını gösterir. Varsayılan değer true'tur"
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/parsehtmltagincell/
---
## HtmlSaveOptions.ParseHtmlTagInCell property

Hücredeki html etiketi (örneğin `<div></div>`) hücre değeri olarak ayrıştırılsın mı yoksa olduğu gibi korunsun mu olduğunu gösterir. Varsayılan değer true'tur.

```csharp
public bool ParseHtmlTagInCell { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyParseHtmlTagInCellDemo
    {
        public static void Run()
        {
            // HTML etiketleri içeren örnek verilerle bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // HTML etiketleriyle hücre değerini ayarla
            worksheet.Cells["A1"].PutValue("<b>Bold Text</b> and <i>Italic Text</i>");
            
            // HTML kaydetme seçeneklerini oluştur ve HTML etiket ayrıştırmayı etkinleştir
            HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions(SaveFormat.Html);
            htmlSaveOptions.ParseHtmlTagInCell = true;
            
            // HTML etiketleri ayrıştırılmış şekilde çalışma kitabını kaydet
            workbook.Save("output.html", htmlSaveOptions);
            
            Console.WriteLine("HTML saved with ParseHtmlTagInCell enabled.");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


