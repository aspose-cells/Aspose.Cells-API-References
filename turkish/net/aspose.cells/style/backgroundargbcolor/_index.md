---
title: "Style.BackgroundArgbColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. 32 bit ARGB değeriyle arka plan rengini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/style/backgroundargbcolor/
---
## Style.BackgroundArgbColor property

32-bit ARGB değeriyle arka plan rengini alır ve ayarlar.

```csharp
public int BackgroundArgbColor { get; set; }
```

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyBackgroundArgbColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Style style = cell.GetStyle();
            style.BackgroundArgbColor = Color.Yellow.ToArgb();
            style.Pattern = BackgroundType.Solid;
            
            cell.SetStyle(style);
            cell.PutValue("Sample Text with Yellow Background");
            
            workbook.Save("BackgroundArgbColorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


