---
title: "Style.BackgroundThemeColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. Arka plan tema rengini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/style/backgroundthemecolor/
---
## Style.BackgroundThemeColor property

Arka plan tema rengini alır ve ayarlar.

```csharp
public ThemeColor BackgroundThemeColor { get; set; }
```

### Açıklamalar

Arka plan rengi bir tema rengi değilse, NULL döndürülecektir.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyBackgroundThemeColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Bir stil oluştur ve arka plan tema rengini ayarla
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            
            ThemeColor themeColor = new ThemeColor(ThemeColorType.Accent2, 0.5);
            style.BackgroundThemeColor = themeColor;

            // Stili bir hücreye uygula
            cells["A1"].SetStyle(style);

            // Arka plan tema rengini doğrula
            ThemeColor retrievedColor = cells["A1"].GetStyle().BackgroundThemeColor;
            Console.WriteLine("Background Theme Color Type: " + retrievedColor.ColorType);
            Console.WriteLine("Background Theme Color Tint: " + retrievedColor.Tint);
        }
    }
}
```

### Ayrıca Bakınız

* class [ThemeColor](../../themecolor/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


