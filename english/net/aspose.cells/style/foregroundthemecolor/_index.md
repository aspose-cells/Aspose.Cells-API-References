---
title: Style.ForegroundThemeColor
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets and sets the foreground theme color
type: docs
url: /net/aspose.cells/style/foregroundthemecolor/
---
## Style.ForegroundThemeColor property

Gets and sets the foreground theme color.

```csharp
public ThemeColor ForegroundThemeColor { get; set; }
```

### Remarks

If the foreground color is not a theme color, NULL will be returned.

### Examples

```csharp
// Called: style.ForegroundThemeColor = new ThemeColor(ThemeColorType.Background2, -0.75);
public static void Property_ForegroundThemeColor()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Adding a value to cell A1
            cells["A1"].PutValue("Hello World");

            // Getting the style of cell A1
            Style style = cells["A1"].GetStyle();

            // Set ThemeColorType.Text2 color type with 40% lighten as the font color.
            style.Font.ThemeColor = new ThemeColor(ThemeColorType.Text2, 0.4);
            style.Pattern = BackgroundType.Solid;

            // Set ThemeColorType.Background2 color type with 75% darken as the foreground color
            style.ForegroundThemeColor = new ThemeColor(ThemeColorType.Background2, -0.75);

            // Applying the style to cell A1
            cells["A1"].SetStyle(style);

            // Saving the Excel file
            workbook.Save("ThemeColorExample.xlsx");
        }
```

### See Also

* class [ThemeColor](../../themecolor/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


