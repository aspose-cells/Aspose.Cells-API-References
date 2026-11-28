---
title: "Enum HtmlVersion"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.HtmlVersion enum. HTML formatlarına kaydederken kullanılan HTML sürümünü gösterir."
type: docs
url: /tr/net/aspose.cells/htmlversion/
---
## HtmlVersion enumeration

HTML formatlarına kaydedilirken kullanılan HTML sürümünü gösterir.

```csharp
public enum HtmlVersion
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Default | `0` | Belgeyi MS Excel dışa aktarma HTML'sine uygun olarak kaydedin. |
| XHtml | `1` | Belgeyi XHTML 1.0 Transitional standardına uygun olarak kaydeder. |
| Html5 | `2` | Belgeyi HTML 5 standardına uygun olarak kaydeder. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassHtmlVersionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("HTML Version Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates HtmlVersion usage");

            // HTML kaydetme seçenekleri oluştur
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();

            // HTML sürümünü HTML5 olarak ayarlayın.
            saveOptions.HtmlVersion = HtmlVersion.Html5;

            // Çalışma kitabını HTML5 sürümüyle kaydedin.
            workbook.Save("HtmlVersionDemo_Html5.html", saveOptions);

            // HTML sürümünü XHTML olarak değiştirin.
            saveOptions.HtmlVersion = HtmlVersion.XHtml;

            // Çalışma kitabını XHTML sürümüyle kaydedin.
            workbook.Save("HtmlVersionDemo_XHtml.html", saveOptions);

            // HTML sürümünü Varsayılan (MS Excel uyumlu) olarak ayarlayın.
            saveOptions.HtmlVersion = HtmlVersion.Default;

            // Çalışma kitabını Varsayılan sürümle kaydedin.
            workbook.Save("HtmlVersionDemo_Default.html", saveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


