---
title: "Font.ArgbColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Font özelliği. 32 bit ARGB değeriyle rengi alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/font/argbcolor/
---
## Font.ArgbColor property

32-bit ARGB değeriyle rengi alır ve ayarlar.

```csharp
public int ArgbColor { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyArgbColorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere eriş ve farklı yazı tipi renkleriyle değerleri ayarla
            Cell cell1 = worksheet.Cells["A1"];
            cell1.PutValue("Red Text");
            Style style1 = cell1.GetStyle();
            style1.Font.ArgbColor = unchecked((int)0xFFFF0000); // Red
            cell1.SetStyle(style1);

            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue("Blue Text");
            Style style2 = cell2.GetStyle();
            style2.Font.ArgbColor = unchecked((int)0xFF0000FF); // Blue
            cell2.SetStyle(style2);

            Cell cell3 = worksheet.Cells["A3"];
            cell3.PutValue("Green Text");
            Style style3 = cell3.GetStyle();
            style3.Font.ArgbColor = unchecked((int)0xFF00FF00); // Green
            cell3.SetStyle(style3);

            // Renkleri doğrula ve çıktı olarak ver
            Console.WriteLine("Cell A1 Font Color: 0x{0:X8}", worksheet.Cells["A1"].GetStyle().Font.ArgbColor);
            Console.WriteLine("Cell A2 Font Color: 0x{0:X8}", worksheet.Cells["A2"].GetStyle().Font.ArgbColor);
            Console.WriteLine("Cell A3 Font Color: 0x{0:X8}", worksheet.Cells["A3"].GetStyle().Font.ArgbColor);
        }
    }
}
```

### Ayrıca Bakınız

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


