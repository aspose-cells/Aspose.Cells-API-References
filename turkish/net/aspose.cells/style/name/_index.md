---
title: "Style.Name"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. Stil adını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/style/name/
---
## Style.Name property

Stil adını alır veya ayarlar.

```csharp
public string Name { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // İlk adlandırılmış stili oluşturun ve uygulayın
            Style style1 = workbook.CreateStyle();
            style1.Number = 7;
            style1.Name = "Sales";
            worksheet.Cells["A1"].SetStyle(style1);
            worksheet.Cells["A1"].PutValue("Sales Data");
            
            // İkinci adlandırılmış stili oluşturun ve uygulayın
            Style style2 = workbook.CreateStyle();
            style2.Font.Size = 14;
            style2.Font.IsBold = true;
            style2.Font.IsItalic = true;
            style2.Font.Color = System.Drawing.Color.Yellow;
            style2.ForegroundColor = System.Drawing.Color.Blue;
            style2.Pattern = BackgroundType.Solid;
            style2.Name = "Header";
            worksheet.Cells["B1"].SetStyle(style2);
            worksheet.Cells["B1"].PutValue("Header Text");
            
            // Çalışma kitabını kaydedin
            workbook.Save("StylePropertyNameDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


