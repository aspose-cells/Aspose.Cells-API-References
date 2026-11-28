---
title: "FontFileDataInfo sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.FontFileDataInfo sınıfı. Yazı tipi dosyası verilerinin bilgi verilerini temsil eder"
type: docs
url: /tr/net/aspose.cells/fontfiledatainfo/
---
## FontFileDataInfo class

Yazı tipi dosyası verilerinin bilgi verisini temsil eder.

```csharp
public class FontFileDataInfo
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Data](../../aspose.cells/fontfiledatainfo/data/) { get; } | Yazı tipi dosyasının ikili verilerini alır. |
| [FormatType](../../aspose.cells/fontfiledatainfo/formattype/) { get; } | Yazı tipi dosyasının format türünü alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsClassFontFileDataInfoDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek: Yazı tipi dosyası verilerini yükleme
            string fontFilePath = "arial.ttf";
            byte[] fontData = File.ReadAllBytes(fontFilePath);

            // Not: FontFileDataInfo, herkese açık bir yapıcıya sahip olmadığından doğrudan örneklenemez
            // ve özellikleri yalnızca okunur. Gerçek bir senaryoda, bir örnek alırsınız
            // başka bir API yönteminden (örneğin FontConfigs.GetFontFileDataInfo())
            FontFileDataInfo fontInfo = null; // Would be populated by API call in real scenario

            // Bir örnek varsa özelliklerin nasıl kullanılacağını gösterin
            if (fontInfo != null)
            {
                Console.WriteLine("Font format type: " + fontInfo.FormatType);
                Console.WriteLine("Font data length: " + (fontInfo.Data != null ? fontInfo.Data.Length.ToString() : "null"));
            }

            // Workbook ile entegrasyonu gösterin
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A1"].PutValue("Text with custom font");

            // Çalışma kitabını kaydedin
            workbook.Save("FontFileDataInfoDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


