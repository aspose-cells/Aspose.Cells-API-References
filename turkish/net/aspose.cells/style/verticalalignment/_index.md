---
title: "Style.VerticalAlignment"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. Hücredeki metnin dikey hizalama türünü alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/style/verticalalignment/
---
## Style.VerticalAlignment property

Bir hücredeki metnin dikey hizalama türünü alır veya ayarlar.

```csharp
public TextAlignmentType VerticalAlignment { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyVerticalAlignmentDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // A1 hücresine eriş
            Cell cell = worksheet.Cells["A1"];
            
            // Hücre değerini ayarla
            cell.PutValue("Vertical Alignment Demo");
            
            // Hücrenin stiline eriş
            Style style = cell.GetStyle();
            
            // Dikey hizalamayı Üst olarak ayarla
            style.VerticalAlignment = TextAlignmentType.Top;
            cell.SetStyle(style);
            
            // Çalışma kitabını kaydedin
            workbook.Save("VerticalAlignmentDemo.xlsx");
            
            Console.WriteLine("Vertical alignment set to Top for cell A1.");
        }
    }
}
```

### Ayrıca Bakınız

* enum [TextAlignmentType](../../textalignmenttype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


