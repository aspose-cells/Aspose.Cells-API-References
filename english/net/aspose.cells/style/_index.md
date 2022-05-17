---
title: Style
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 5740
url: /net/aspose.cells/style/
---
## Style class

Represents display style of excel document,such as font,color,alignment,border,etc.

```csharp
public class Style
```

## Properties

| Name | Description |
| --- | --- |
| [BackgroundArgbColor](backgroundargbcolor) { get; set; } | Gets and sets the background color with a 32-bit ARGB value. |
| [BackgroundColor](backgroundcolor) { get; set; } | Gets or sets a style's background color. |
| [BackgroundThemeColor](backgroundthemecolor) { get; set; } | Gets and sets the background theme color. |
| [Borders](borders) { get; } | Gets the [`BorderCollection`](../bordercollection) of the style. |
| [CultureCustom](culturecustom) { get; set; } | Gets and sets the culture-dependent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned. |
| [Custom](custom) { get; set; } | Represents the custom number format string of this style object. If the custom number format is not set(For example, the number format is builtin), "" will be returned. |
| [Font](font) { get; } | Gets a [`Font`](./font) object. |
| [ForegroundArgbColor](foregroundargbcolor) { get; set; } | Gets and sets the foreground color with a 32-bit ARGB value. |
| [ForegroundColor](foregroundcolor) { get; set; } | Gets or sets a style's foreground color. |
| [ForegroundThemeColor](foregroundthemecolor) { get; set; } | Gets and sets the foreground theme color. |
| [HasBorders](hasborders) { get; } | Checks whether there are borders have been set for the style. |
| [HorizontalAlignment](horizontalalignment) { get; set; } | Gets or sets the horizontal alignment type of the text in a cell. |
| [IndentLevel](indentlevel) { get; set; } | Represents the indent level for the cell or range. Can only be an integer from 0 to 250. |
| [InvariantCustom](invariantcustom) { get; } | Gets the culture-independent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned. |
| [IsDateTime](isdatetime) { get; } | Indicates whether the number format is a date format. |
| [IsFormulaHidden](isformulahidden) { get; set; } | Represents if the formula will be hidden when the worksheet is protected. |
| [IsGradient](isgradient) { get; set; } | Indicates whether the cell shading is a gradient pattern. |
| [IsJustifyDistributed](isjustifydistributed) { get; set; } | Indicates if the cells justified or distributed alignment should be used on the last line of text. |
| [IsLocked](islocked) { get; set; } | Gets or sets a value indicating whether a cell can be modified or not. |
| [IsPercent](ispercent) { get; } | Indicates whether the number format is a percent format. |
| [IsTextWrapped](istextwrapped) { get; set; } | Gets or sets a value indicating whether the text within a cell is wrapped. |
| [Name](name) { get; set; } | Gets or sets the name of the style. |
| [Number](number) { get; set; } | Gets or sets the display format of numbers and dates. The formatting patterns are different for different regions. |
| [ParentStyle](parentstyle) { get; } | Gets the parent style of this style. |
| [Pattern](pattern) { get; set; } | Gets or sets the cell background pattern type. |
| [QuotePrefix](quoteprefix) { get; set; } | Indicates whether the cell's value starts with single quote mark. |
| [RotationAngle](rotationangle) { get; set; } | Represents text rotation angle. |
| [ShrinkToFit](shrinktofit) { get; set; } | Represents if text automatically shrinks to fit in the available column width. |
| [TextDirection](textdirection) { get; set; } | Represents text reading order. |
| [VerticalAlignment](verticalalignment) { get; set; } | Gets or sets the vertical alignment type of the text in a cell. |

## Methods

| Name | Description |
| --- | --- |
| [Copy](copy)(Style) | Copies data from another style object |
| override [Equals](equals)(object) | Determines whether two Style instances are equal. |
| override [GetHashCode](gethashcode)() | Serves as a hash function for a Style object. |
| [GetTwoColorGradient](gettwocolorgradient)(out Color, out Color, out GradientStyleType, out int) | Get the two-color gradient setting. |
| [IsModified](ismodified)(StyleModifyFlag) | Checks whether the specified properties of the style have been modified. Used for style of ConditionalFormattings to check whether the specified properties of this style should be used when applying the ConditionalFormattings on a cell. |
| [SetBorder](setborder)(BorderType, CellBorderType, Color) | Sets the borders of the style. |
| [SetCustom](setcustom)(string, bool) | Sets the Custom number format string of a cell. |
| [SetPatternColor](setpatterncolor)(BackgroundType, Color, Color) | Sets the background color. |
| [SetTwoColorGradient](settwocolorgradient)(Color, Color, GradientStyleType, int) | Sets the specified fill to a two-color gradient. |
| [Update](update)() | Apply the named style to the styles of the cells which use this named style. It works like clicking the "ok" button after you finished modifying the style. Only applies for named style. |

### Examples

```csharp
[C#]
Workbook workbook = new Workbook();

WorksheetCollection sheets = workbook.Worksheets;
Cell cell = sheets[0].Cells["A1"];
Style style =  cell.GetStyle();
style.Font.Name = "Times New Roman";
style.Font.Color = Color.Blue;
cell.SetStyle(style);
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
