---
title: Style
second_title: Aspose.Cells for .NET API Reference
description: Represents display style of excel documentsuch as fontcoloralignmentborderetc. The Style object contains all style attributes font number format alignment and so on as properties.
type: docs
weight: 5780
url: /net/aspose.cells/style/
---
## Style class

Represents display style of excel document,such as font,color,alignment,border,etc. The Style object contains all style attributes (font, number format, alignment, and so on) as properties.

```csharp
public class Style
```

## Constructors

| Name | Description |
| --- | --- |
| [Style](style)() | (**Obsolete.**) Initializes a new instance of the [`Style`](../style) class. |

## Properties

| Name | Description |
| --- | --- |
| [BackgroundArgbColor](../../aspose.cells/style/backgroundargbcolor) { get; set; } | Gets and sets the background color with a 32-bit ARGB value. |
| [BackgroundColor](../../aspose.cells/style/backgroundcolor) { get; set; } | Gets or sets a style's background color. |
| [BackgroundThemeColor](../../aspose.cells/style/backgroundthemecolor) { get; set; } | Gets and sets the background theme color. |
| [Borders](../../aspose.cells/style/borders) { get; } | Gets the [`BorderCollection`](../bordercollection) of the style. |
| [CultureCustom](../../aspose.cells/style/culturecustom) { get; set; } | Gets and sets the culture-dependent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned. |
| [Custom](../../aspose.cells/style/custom) { get; set; } | Represents the custom number format string of this style object. If the custom number format is not set(For example, the number format is builtin), "" will be returned. |
| [Font](../../aspose.cells/style/font) { get; } | Gets a [`Font`](./font) object. |
| [ForegroundArgbColor](../../aspose.cells/style/foregroundargbcolor) { get; set; } | Gets and sets the foreground color with a 32-bit ARGB value. |
| [ForegroundColor](../../aspose.cells/style/foregroundcolor) { get; set; } | Gets or sets a style's foreground color. |
| [ForegroundThemeColor](../../aspose.cells/style/foregroundthemecolor) { get; set; } | Gets and sets the foreground theme color. |
| [HasBorders](../../aspose.cells/style/hasborders) { get; } | Checks whether there are borders have been set for the style. |
| [HorizontalAlignment](../../aspose.cells/style/horizontalalignment) { get; set; } | Gets or sets the horizontal alignment type of the text in a cell. |
| [IndentLevel](../../aspose.cells/style/indentlevel) { get; set; } | Represents the indent level for the cell or range. Can only be an integer from 0 to 250. |
| [InvariantCustom](../../aspose.cells/style/invariantcustom) { get; } | Gets the culture-independent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned. |
| [IsDateTime](../../aspose.cells/style/isdatetime) { get; } | Indicates whether the number format is a date format. |
| [IsFormulaHidden](../../aspose.cells/style/isformulahidden) { get; set; } | Represents if the formula will be hidden when the worksheet is protected. |
| [IsGradient](../../aspose.cells/style/isgradient) { get; set; } | Indicates whether the cell shading is a gradient pattern. |
| [IsJustifyDistributed](../../aspose.cells/style/isjustifydistributed) { get; set; } | Indicates if the cells justified or distributed alignment should be used on the last line of text. |
| [IsLocked](../../aspose.cells/style/islocked) { get; set; } | Gets or sets a value indicating whether a cell can be modified or not. |
| [IsPercent](../../aspose.cells/style/ispercent) { get; } | Indicates whether the number format is a percent format. |
| [IsTextWrapped](../../aspose.cells/style/istextwrapped) { get; set; } | Gets or sets a value indicating whether the text within a cell is wrapped. |
| [Name](../../aspose.cells/style/name) { get; set; } | Gets or sets the name of the style. |
| [Number](../../aspose.cells/style/number) { get; set; } | Gets or sets the display format of numbers and dates. The formatting patterns are different for different regions. |
| [ParentStyle](../../aspose.cells/style/parentstyle) { get; } | Gets the parent style of this style. |
| [Pattern](../../aspose.cells/style/pattern) { get; set; } | Gets or sets the cell background pattern type. |
| [QuotePrefix](../../aspose.cells/style/quoteprefix) { get; set; } | Indicates whether the cell's value starts with single quote mark. |
| [RotationAngle](../../aspose.cells/style/rotationangle) { get; set; } | Represents text rotation angle. |
| [ShrinkToFit](../../aspose.cells/style/shrinktofit) { get; set; } | Represents if text automatically shrinks to fit in the available column width. |
| [TextDirection](../../aspose.cells/style/textdirection) { get; set; } | Represents text reading order. |
| [VerticalAlignment](../../aspose.cells/style/verticalalignment) { get; set; } | Gets or sets the vertical alignment type of the text in a cell. |

## Methods

| Name | Description |
| --- | --- |
| [Copy](../../aspose.cells/style/copy)(Style) | Copies data from another style object |
| override [Equals](../../aspose.cells/style/equals)(object) | Determines whether two Style instances are equal. |
| override [GetHashCode](../../aspose.cells/style/gethashcode)() | Serves as a hash function for a Style object. |
| [GetTwoColorGradient](../../aspose.cells/style/gettwocolorgradient)(out Color, out Color, out GradientStyleType, out int) | Get the two-color gradient setting. |
| [IsModified](../../aspose.cells/style/ismodified)(StyleModifyFlag) | Checks whether the specified properties of the style have been modified. Used for style of ConditionalFormattings to check whether the specified properties of this style should be used when applying the ConditionalFormattings on a cell. |
| [SetBorder](../../aspose.cells/style/setborder)(BorderType, CellBorderType, Color) | Sets the borders of the style. |
| [SetCustom](../../aspose.cells/style/setcustom)(string, bool) | Sets the Custom number format string of a cell. |
| [SetPatternColor](../../aspose.cells/style/setpatterncolor)(BackgroundType, Color, Color) | Sets the background color. |
| [SetTwoColorGradient](../../aspose.cells/style/settwocolorgradient)(Color, Color, GradientStyleType, int) | Sets the specified fill to a two-color gradient. |
| [Update](../../aspose.cells/style/update)() | Apply the named style to the styles of the cells which use this named style. It works like clicking the "ok" button after you finished modifying the style. Only applies for named style. |

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
