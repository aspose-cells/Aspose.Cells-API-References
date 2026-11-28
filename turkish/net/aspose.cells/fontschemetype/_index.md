---
title: "Enum FontSchemeType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.FontSchemeType enum. Yazı tipinin şema türünü temsil eder."
type: docs
url: /tr/net/aspose.cells/fontschemetype/
---
## FontSchemeType enumeration

Yazı tipinin şema türünü temsil eder.

```csharp
public enum FontSchemeType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Yok |
| Major | `1` | Ana şema. |
| Minor | `2` | Alt şema. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontSchemeTypeDemo
    {
        public static void FontSchemeTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            // İlk çalışma sayfasının referansını alın.
            Worksheet worksheet = workbook.Worksheets[0];
            // Çalışma sayfasından "A1" hücresine erişme
            Cell cell = worksheet.Cells["A1"];
            // "A1" hücresine bir değer ekleme
            cell.PutValue("Hello Aspose!");

            // Hücre stilinin yazı tipine erişin.
            Aspose.Cells.Font font = cell.GetStyle().Font;

            // Yazı tipi şema türünü Major olarak ayarlama.
            font.SchemeType = FontSchemeType.Major;

            // Demonstrasyon için diğer yazı tipi özelliklerini ayarlama.
            font.Name = "Arial";
            font.Size = 14;
            font.Color = System.Drawing.Color.Blue;

            // Çalışma kitabını kaydedin
            workbook.Save("FontSchemeTypeExample.xlsx");
            workbook.Save("FontSchemeTypeExample.pdf");
            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


