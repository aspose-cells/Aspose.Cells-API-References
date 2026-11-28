---
title: "Font.SchemeType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Font özelliği. Fontun şema tipini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/font/schemetype/
---
## Font.SchemeType property

Yazı tipinin şema türünü alır ve ayarlar.

```csharp
public FontSchemeType SchemeType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertySchemeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            Font font = cell.GetStyle().Font;
            font.SchemeType = FontSchemeType.Minor;
            font.Name = "Calibri";
            font.Size = 12;

            workbook.Save("FontSchemeTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [FontSchemeType](../../fontschemetype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


