---
title: "Font.Size"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Font özelliği. Yazı tipinin boyutunu alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/font/size/
---
## Font.Size property

Yazı tipinin boyutunu alır veya ayarlar.

```csharp
public int Size { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertySizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Farklı yazı tipi boyutlarıyla metin ayarla
            Cell cell1 = worksheet.Cells["A1"];
            cell1.Value = "Text with size 12";
            Style style1 = workbook.CreateStyle();
            style1.Font.Size = 12;
            cell1.SetStyle(style1);

            Cell cell2 = worksheet.Cells["A3"];
            cell2.Value = "Text with size 16";
            Style style2 = workbook.CreateStyle();
            style2.Font.Size = 16;
            cell2.SetStyle(style2);

            // Çalışma kitabını kaydedin
            workbook.Save("FontSizeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


