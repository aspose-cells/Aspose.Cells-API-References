---
title: "Style.IsNumberFormatApplied"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. Sayı biçimlendirmesinin uygulanıp uygulanmayacağını belirtir"
type: docs
url: /tr/net/aspose.cells/style/isnumberformatapplied/
---
## Style.IsNumberFormatApplied property

Sayı biçimlendirmesinin uygulanıp uygulanmayacağını belirt.

```csharp
public bool IsNumberFormatApplied { get; set; }
```

### Açıklamalar

Yalnızca adlandırılmış stil için.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsNumberFormatAppliedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Sayı biçimiyle bir stil oluştur
            Style style = workbook.CreateStyle();
            style.Number = 14; // Format as "m/d/yyyy"
            style.IsNumberFormatApplied = true;
            
            // Stili bir hücreye uygula
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            
            // Sayı biçiminin uygulandığını doğrula
            Console.WriteLine("IsNumberFormatApplied: " + style.IsNumberFormatApplied);
            Console.WriteLine("Cell value format: " + cell.GetDisplayStyle().Number);
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


