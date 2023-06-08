---
title: Class ThemeColor
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ThemeColor class. Represents a theme color
type: docs
url: /net/aspose.cells/themecolor/
---
## ThemeColor class

Represents a theme color.

```csharp
public class ThemeColor
```

## Constructors

| Name | Description |
| --- | --- |
| [ThemeColor](themecolor/)(ThemeColorType, double) |  |

## Properties

| Name | Description |
| --- | --- |
| [ColorType](../../aspose.cells/themecolor/colortype/) { get; set; } | Gets and sets the theme type. |
| [Tint](../../aspose.cells/themecolor/tint/) { get; set; } | Gets and sets the tint value. |

### Examples

```csharp

[C#]

//Instantiating a Workbook object
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
cells["A1"].PutValue("Hello World");
Style style = cells["A1"].GetStyle();
//Set ThemeColorType.Text2 color type with 40% lighten as the font color.
style.Font.ThemeColor = new ThemeColor(ThemeColorType.Text2, 0.4);
style.Pattern = BackgroundType.Solid;
//Set ThemeColorType.Background2 color type with 75% darken as the foreground color
style.ForegroundThemeColor = new ThemeColor(ThemeColorType.Background2, -0.75);
cells["A1"].SetStyle(style);
//Saving the Excel file
workbook.Save("book1.xlsx");

[Visual Basic]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()
Dim cells As Cells = workbook.Worksheets(0).Cells
cells("A1").PutValue("Hello World")
'Get the cell style
Dim style As Style = cells("A1").GetStyle()
'Set ThemeColorType.Text2 color type with 40% lighten as the font color.
Style.Font.ThemeColor = New ThemeColor(ThemeColorType.Text2, 0.4)
Style.Pattern = BackgroundType.Solid
'Set ThemeColorType.Background2 color type with 75% darken as the foreground color
style.ForegroundThemeColor = New ThemeColor(ThemeColorType.Background2, -0.75)
'Set the cell style
cells("A1").SetStyle(style)
'Saving the Excel file
Workbook.Save("book1.xlsx")
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


