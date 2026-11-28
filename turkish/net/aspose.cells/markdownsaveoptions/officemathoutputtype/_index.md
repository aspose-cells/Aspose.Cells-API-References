---
title: "MarkdownSaveOptions.OfficeMathOutputType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MarkdownSaveOptions özelliği. OfficeMath nesnelerinin Markdown'a nasıl dışa aktarıldığını gösterir. Varsayılan değer Image"
type: docs
url: /tr/net/aspose.cells/markdownsaveoptions/officemathoutputtype/
---
## MarkdownSaveOptions.OfficeMathOutputType property

OfficeMath nesnelerinin Markdown'a nasıl dışa aktarıldığını gösterir, varsayılan değer Görüntü'dür.

```csharp
public HtmlOfficeMathOutputType OfficeMathOutputType { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyOfficeMathOutputTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // OfficeMath içerebilecek bir formül dahil olmak üzere örnek veri ekle
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].Formula = "=SQRT(16)";

            try
            {
                // Markdown kaydetme seçeneklerini oluştur
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // OfficeMathOutputType'ın mevcut değerini göster
                Console.WriteLine("Current OfficeMathOutputType: " + saveOptions.OfficeMathOutputType);

                // OfficeMathOutputType'ı MathML olarak ayarla
                saveOptions.OfficeMathOutputType = HtmlOfficeMathOutputType.MathML;
                Console.WriteLine("Changed OfficeMathOutputType to: " + saveOptions.OfficeMathOutputType);

                // Çalışma kitabını MathML çıktı türüyle kaydet
                workbook.Save("OfficeMathOutputType_MathML.md", saveOptions);

                // Çıktı türünü Image olarak değiştir
                saveOptions.OfficeMathOutputType = HtmlOfficeMathOutputType.Image;
                Console.WriteLine("Changed OfficeMathOutputType to: " + saveOptions.OfficeMathOutputType);

                // Çalışma kitabını Image çıktı türüyle kaydet
                workbook.Save("OfficeMathOutputType_Image.md", saveOptions);

                Console.WriteLine("OfficeMathOutputType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [HtmlOfficeMathOutputType](../../htmlofficemathoutputtype/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


