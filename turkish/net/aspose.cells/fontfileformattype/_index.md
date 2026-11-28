---
title: "Enum FontFileFormatType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.FontFileFormatType enum. Yazı tipi formatı türünü temsil eder"
type: docs
url: /tr/net/aspose.cells/fontfileformattype/
---
## FontFileFormatType enumeration

Yazı tipi formatı türünü temsil eder.

```csharp
public enum FontFileFormatType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Unknown | `0` | Bilinmeyen yazı tipi formatı türü. |
| Ttf | `1` | TTF yazı tipi formatı türü. |
| Otf | `2` | OTF yazı tipi formatı türü. |
| Ttc | `3` | TTC yazı tipi formatı türü. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassFontFileFormatTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir hücreye erişin ve stilini ayarlayın
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Font Format Type Demo");
            Style style = cell.GetStyle();

            // FontFileFormatType kullanımını gösterin
            FontFileFormatType fontFormat = FontFileFormatType.Ttf;
            Console.WriteLine("Selected font format: " + fontFormat.ToString());

            // Yazı tipi ayarlarını uygulayın
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            cell.SetStyle(style);

            // Yazı tipi formatı uyumluluğunu kontrol edin
            if (fontFormat == FontFileFormatType.Ttf)
            {
                Console.WriteLine("Using TrueType font format");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("FontFileFormatTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


