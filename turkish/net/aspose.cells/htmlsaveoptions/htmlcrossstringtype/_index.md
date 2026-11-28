---
title: "HtmlSaveOptions.HtmlCrossStringType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Bir çapraz hücre dizesinin, Excel dosyasını html formatında kaydederken MS Excel gibi görüntülenip görüntülenmeyeceğini gösterir. Varsayılan değer Default olduğundan, çapraz hücre dizeleri için Aspose.Cells ve MS Excel tarafından oluşturulan html dosyaları arasında çok az fark vardır. Ancak büyük html dosyaları oluştururken değeri Cross olarak ayarlamak, Default ya da Fit2Cell olarak ayarlamaktan birkaç kat daha hızlı olur."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/htmlcrossstringtype/
---
## HtmlSaveOptions.HtmlCrossStringType property

Excel dosyasını html formatında kaydederken çapraz hücre dizesinin MS Excel ile aynı şekilde görüntülenip görüntülenmeyeceğini gösterir. Varsayılan değer "Default"'tır, bu nedenle çapraz hücre dizileri için Aspose.Cells ve MS Excel tarafından oluşturulan html dosyaları arasında çok az fark vardır. Ancak büyük html dosyaları oluştururken, değeri "Cross" olarak ayarlamak, "Default" veya "Fit2Cell"'e göre birkaç kat daha hızlı olur.

```csharp
public HtmlCrossType HtmlCrossStringType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHtmlCrossStringTypeDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çapraz dize davranışını gösterecek örnek veri ekle
            worksheet.Cells["A1"].PutValue("Left Content");
            worksheet.Cells["B1"].PutValue("Right Content");
            
            // Hücre stillerini al ve değiştir
            Style styleA1 = worksheet.Cells["A1"].GetStyle();
            styleA1.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            worksheet.Cells["A1"].SetStyle(styleA1);
            
            Style styleB1 = worksheet.Cells["B1"].GetStyle();
            styleB1.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            worksheet.Cells["B1"].SetStyle(styleB1);

            // HTML kaydetme seçeneklerini yapılandır
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.HtmlCrossStringType = HtmlCrossType.CrossHideRight;

            // Çalışma kitabını HTML olarak kaydedin
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML file saved with CrossHideRight option.");
        }
    }
}
```

### Ayrıca Bakınız

* enum [HtmlCrossType](../../htmlcrosstype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


