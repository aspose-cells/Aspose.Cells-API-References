---
title: "Style.ForegroundColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. Bir stilin ön plan rengini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/style/foregroundcolor/
---
## Style.ForegroundColor property

Bir stilin ön plan rengini alır veya ayarlar.

```csharp
public Color ForegroundColor { get; set; }
```

### Açıklamalar

Color.Empty döndürülürse renk ayarının olmadığı anlamına gelir.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyForegroundColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            Style style = workbook.CreateStyle();
            style.ForegroundColor = Color.Green;
            style.Pattern = BackgroundType.Solid;
            
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            
            Console.WriteLine("ForegroundColor set to: " + style.ForegroundColor);
            
            workbook.Save("ForegroundColorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


