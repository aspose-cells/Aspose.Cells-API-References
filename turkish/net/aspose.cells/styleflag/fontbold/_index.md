---
title: "StyleFlag.FontBold"
second_title: "Aspose.Cells için .NET API Referansı"
description: "StyleFlag özelliği. Kalın yazı tipi ayarı uygulanacak"
type: docs
url: /tr/net/aspose.cells/styleflag/fontbold/
---
## StyleFlag.FontBold property

Yazı tipi kalın ayarı uygulanacak.

```csharp
public bool FontBold { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyFontBoldDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Kalın bir stil oluştur
            Style boldStyle = workbook.CreateStyle();
            boldStyle.Font.IsBold = true;

            // Yalnızca FontBold için StyleFlag kullanarak satır 2'ye kalın stil uygula
            worksheet.Cells.ApplyRowStyle(1, boldStyle, new StyleFlag { FontBold = true });

            // Stili göstermek için hücreye değer koy
            worksheet.Cells[1, 0].PutValue("Bold Text");

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");

            Console.WriteLine("FontBold property demo completed successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


