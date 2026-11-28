---
title: "Font.Underline"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Yazı tipi özelliği. Yazı tipinin alt çizgi türünü alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/font/underline/
---
## Font.Underline property

Yazı tipinin alt çizgi tipini alır veya ayarlar.

```csharp
public FontUnderlineType Underline { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyUnderlineDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Hücreye eriş ve alt çizgi stilini ayarla
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Sample Underlined Text");
            
            // Stili al ve yazı tipi özelliklerini değiştir
            Style style = cell.GetStyle();
            style.Font.Underline = FontUnderlineType.Single;
            cell.SetStyle(style);

            // Çalışma kitabını kaydedin
            workbook.Save("FontUnderlineDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [FontUnderlineType](../../fontunderlinetype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


