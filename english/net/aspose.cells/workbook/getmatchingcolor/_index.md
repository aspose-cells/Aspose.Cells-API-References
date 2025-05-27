---
title: Workbook.GetMatchingColor
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Find best matching Color in current palette
type: docs
url: /net/aspose.cells/workbook/getmatchingcolor/
---
## Workbook.GetMatchingColor method

Find best matching Color in current palette.

```csharp
public Color GetMatchingColor(Color rawColor)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rawColor | Color | Raw color. |

### Return Value

Best matching color.

### Examples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodGetMatchingColorWithColorDemo
    {
        public static void Run()
        {
            // Create a workbook
            Workbook workbook = new Workbook();
            
            // Check if color exists in palette
            Console.WriteLine("Is Red in palette: " + workbook.IsColorInPalette(Color.Red));
            Color testColor = Color.FromArgb(255, 123, 123, 123);
            Console.WriteLine("Is custom color in palette: " + workbook.IsColorInPalette(testColor));

            // Get matching color from palette
            Color matchedColor = workbook.GetMatchingColor(testColor);
            Console.WriteLine($"Original color: R={testColor.R}, G={testColor.G}, B={testColor.B}");
            Console.WriteLine($"Matched color: R={matchedColor.R}, G={matchedColor.G}, B={matchedColor.B}");

            // Create a custom theme
            Color[] themeColors = new Color[12];
            for (int i = 0; i < themeColors.Length; i++)
            {
                themeColors[i] = Color.FromArgb(255, 128 + i, 128 + i, 128 + i);
            }
            workbook.CustomTheme("CustomTheme", themeColors);

            // Get theme color
            Color themeColor = workbook.GetThemeColor(ThemeColorType.FollowedHyperlink);
            Console.WriteLine($"Theme color: R={themeColor.R}, G={themeColor.G}, B={themeColor.B}");
        }
    }
}
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


