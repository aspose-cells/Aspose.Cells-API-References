---
title: "Font.IsItalic"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Yazı tipi özelliği. Yazı tipinin italik olup olmadığını gösteren bir değeri alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/font/isitalic/
---
## Font.IsItalic property

Yazı tipinin italik olup olmadığını gösteren bir değeri alır veya ayarlar.

```csharp
public bool IsItalic { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsItalicDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Varsayılan stile eriş
            Style style = workbook.DefaultStyle;
            
            // IsItalic dahil olmak üzere yazı tipi özelliklerini ayarla
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.Font.IsItalic = true;
            
            // Stili A1 hücresine uygula
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Italic Text Example");
            
            // Çalışma kitabını kaydedin
            workbook.Save("FontPropertyIsItalicDemo.xlsx");
            
            // İtalik özelliğini doğrula
            Console.WriteLine("Font is italic: " + cell.GetStyle().Font.IsItalic);
        }
    }
}
```

### Ayrıca Bakınız

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


