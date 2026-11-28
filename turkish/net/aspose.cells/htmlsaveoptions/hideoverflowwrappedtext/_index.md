---
title: "HtmlSaveOptions.HideOverflowWrappedText"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Hücre biçimi metni kaydıracak şekilde ayarlandığında taşan metnin gizlenip gizlenmeyeceğini gösterir. Varsayılan değer false."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/hideoverflowwrappedtext/
---
## HtmlSaveOptions.HideOverflowWrappedText property

Hücre biçimi satır kaydırma olarak ayarlandığında taşan metnin gizlenip gizlenmeyeceğini gösterir. Varsayılan değer false.

```csharp
public bool HideOverflowWrappedText { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHideOverflowWrappedTextDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // A1 hücresine örnek metin ayarlayın
            worksheet.Cells["A1"].PutValue("This is a long text that should wrap and hide overflow when exported to HTML");
            
            // Metin kaydırma ile stil oluşturun ve uygulayın
            Style style = workbook.CreateStyle();
            style.IsTextWrapped = true;
            StyleFlag flag = new StyleFlag();
            flag.WrapText = true;
            
            // Hücre koleksiyonunu alın ve stili uygulayın
            Cells cells = worksheet.Cells;
            cells["A1"].SetStyle(style, flag);
            
            // Metnin kaydırılmasını sağlamak için sütun genişliğini ayarlayın
            cells.SetColumnWidth(0, 10);
            
            // HTML kaydetme seçeneklerini oluşturun ve HideOverflowWrappedText'i ayarlayın
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.HideOverflowWrappedText = true;
            
            // Çalışma kitabını HTML seçenekleriyle kaydet
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("File saved with HideOverflowWrappedText: " + outputPath);
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


