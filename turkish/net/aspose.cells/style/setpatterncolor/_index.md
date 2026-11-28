---
title: "Style.SetPatternColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style yöntemi. Arka plan rengini ayarlar"
type: docs
url: /tr/net/aspose.cells/style/setpatterncolor/
---
## Style.SetPatternColor method

Arka plan rengini ayarlar.

```csharp
public void SetPatternColor(BackgroundType pattern, Color color1, Color color2)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| desen | BackgroundType | Desen. |
| color1 | Color | Ön plan rengi. |
| color2 | Color | Arka plan rengi. Yalnızca desen BackgroundType.None ve BackgroundType.Solid olmadığında çalışır. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleMethodSetPatternColorWithBackgroundTypeColorColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Style style = cell.GetStyle();
            style.SetPatternColor(BackgroundType.Solid, Color.Red, Color.Blue);
            cell.SetStyle(style);
            
            workbook.Save("SetPatternColorDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* enum [BackgroundType](../../backgroundtype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


