---
title: "Style.Pattern"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. Hücre arka planı desen tipini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/style/pattern/
---
## Style.Pattern property

Hücre arka planı desen türünü alır veya ayarlar.

```csharp
public BackgroundType Pattern { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyPatternDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Hücreye eriş ve stilini al
            Cell cell = cells[0, 0];
            Style style = cell.GetStyle();
            
            // Deseni ve ön plan rengini ayarla
            style.Pattern = BackgroundType.Gray50;
            style.ForegroundColor = System.Drawing.Color.LightGray;
            
            // Stili hücreye uygulayın
            cell.SetStyle(style);
            
            // Çalışma kitabını kaydedin
            workbook.Save("PatternPropertyDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [BackgroundType](../../backgroundtype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


