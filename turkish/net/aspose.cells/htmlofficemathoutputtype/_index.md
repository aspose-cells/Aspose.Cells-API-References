---
title: "Enum HtmlOfficeMathOutputType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.HtmlOfficeMathOutputType enum. OfficeMath'i HTML'e nasıl dışa aktarılacağını temsil eder"
type: docs
url: /tr/net/aspose.cells/htmlofficemathoutputtype/
---
## HtmlOfficeMathOutputType enumeration

OfficeMath'i HTML'ye nasıl dışa aktarılacağını temsil eder.

```csharp
public enum HtmlOfficeMathOutputType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Image | `0` | OfficeMath'i &lt;img&gt; etiketiyle belirtilen görüntü olarak HTML'e dönüştürür. |
| MathML | `1` | OfficeMath'i MathML kullanarak HTML'e dönüştürür. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class CellsClassHtmlOfficeMathOutputTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // OfficeMath'i A1 hücresine ekle
            worksheet.Cells["A1"].PutValue("=SUM(1,2)");
            
            // HTML kaydetme seçenekleri oluştur
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // OfficeMath çıktı türünü Görüntü olarak ayarla
            saveOptions.OfficeMathOutputMode = HtmlOfficeMathOutputType.Image;
            
            // Görüntü çıktı türüyle kaydet
            workbook.Save("HtmlOfficeMathOutputType_Image.html", saveOptions);
            
            // Çıktı türünü MathML olarak değiştir
            saveOptions.OfficeMathOutputMode = HtmlOfficeMathOutputType.MathML;
            
            // MathML çıktı türüyle kaydet
            workbook.Save("HtmlOfficeMathOutputType_MathML.html", saveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


