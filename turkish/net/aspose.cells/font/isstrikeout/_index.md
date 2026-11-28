---
title: "Font.IsStrikeout"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Font özelliği. Fontun tek çizgi üzeri olup olmadığını belirten bir değeri alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/font/isstrikeout/
---
## Font.IsStrikeout property

Yazı tipinin tek çizgiyle üzeri çizili olup olmadığını gösteren bir değeri alır veya ayarlar.

```csharp
public bool IsStrikeout { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsStrikeoutDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Yöntem 1: Çizgi üzeri özelliğini doğrudan stil üzerinden ayarla
            Cell cell1 = worksheet.Cells["A1"];
            Style style1 = cell1.GetStyle();
            style1.Font.IsStrikeout = true;
            cell1.SetStyle(style1);
            cell1.PutValue("Strikeout Text (Style)");
            
            // Yöntem 2: Çizgi üzeri özelliğini HTML üzerinden ayarla
            Cell cell2 = worksheet.Cells["A2"];
            cell2.HtmlString = "<s>Strikeout Text (HTML)</s>";
            
            // Çizgi üzeri özelliğini doğrula
            Console.WriteLine("A1 IsStrikeout: " + cell1.GetStyle().Font.IsStrikeout);
            Console.WriteLine("A2 IsStrikeout: " + cell2.GetStyle().Font.IsStrikeout);
            
            // Doğrulama için kaydet
            workbook.Save("FontStrikeoutDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


