---
title: Class TextOptions
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.Texts.TextOptions class. Represents the text options
type: docs
url: /net/aspose.cells.drawing.texts/textoptions/
---
## TextOptions class

Represents the text options.

```csharp
public class TextOptions : Font
```

## Properties

| Name | Description |
| --- | --- |
| [ArgbColor](../../aspose.cells/font/argbcolor/) { get; set; } | Gets and sets the color with a 32-bit ARGB value.(Inherited from [`Font`](../../aspose.cells/font/).) |
| [CapsType](../../aspose.cells.drawing.texts/textoptions/capstype/) { get; set; } | Gets and sets the text caps type. |
| [Charset](../../aspose.cells/font/charset/) { get; set; } | Represent the character set.(Inherited from [`Font`](../../aspose.cells/font/).) |
| [Color](../../aspose.cells/font/color/) { get; set; } | Gets or sets the Color of the font.(Inherited from [`Font`](../../aspose.cells/font/).) |
| [DoubleSize](../../aspose.cells/font/doublesize/) { get; set; } | Gets and sets the double size of the font.(Inherited from [`Font`](../../aspose.cells/font/).) |
| [FarEastName](../../aspose.cells.drawing.texts/textoptions/fareastname/) { get; set; } | Gets and sets the FarEast name. |
| [Fill](../../aspose.cells.drawing.texts/textoptions/fill/) { get; } | Represents the fill format of the text. |
| [IsBold](../../aspose.cells/font/isbold/) { get; set; } | Gets or sets a value indicating whether the font is bold.(Inherited from [`Font`](../../aspose.cells/font/).) |
| [IsItalic](../../aspose.cells/font/isitalic/) { get; set; } | Gets or sets a value indicating whether the font is italic.(Inherited from [`Font`](../../aspose.cells/font/).) |
| [IsNormalizeHeights](../../aspose.cells.drawing.texts/textoptions/isnormalizeheights/) { get; set; } | Indicates whether the normalization of height that is to be applied to the text run. |
| [IsStrikeout](../../aspose.cells/font/isstrikeout/) { get; set; } | Gets or sets a value indicating whether the font is single strikeout.(Inherited from [`Font`](../../aspose.cells/font/).) |
| [IsSubscript](../../aspose.cells/font/issubscript/) { get; set; } | Gets or sets a value indicating whether the font is subscript.(Inherited from [`Font`](../../aspose.cells/font/).) |
| [IsSuperscript](../../aspose.cells/font/issuperscript/) { get; set; } | Gets or sets a value indicating whether the font is super script.(Inherited from [`Font`](../../aspose.cells/font/).) |
| [Kerning](../../aspose.cells.drawing.texts/textoptions/kerning/) { get; set; } | Specifies the minimum font size at which character kerning will occur for this text run. |
| [LanguageCode](../../aspose.cells.drawing.texts/textoptions/languagecode/) { get; set; } | Gets and sets the user interface language. |
| [LatinName](../../aspose.cells.drawing.texts/textoptions/latinname/) { get; set; } | Gets and sets the latin name. |
| override [Name](../../aspose.cells.drawing.texts/textoptions/name/) { get; set; } | Gets and sets the name of the shape. |
| [Outline](../../aspose.cells.drawing.texts/textoptions/outline/) { get; } | Represents the outline format of the text. |
| [SchemeType](../../aspose.cells/font/schemetype/) { get; set; } | Gets and sets the scheme type of the font.(Inherited from [`Font`](../../aspose.cells/font/).) |
| [ScriptOffset](../../aspose.cells/font/scriptoffset/) { get; set; } | Gets and sets the script offset,in unit of percentage(Inherited from [`Font`](../../aspose.cells/font/).) |
| [Shadow](../../aspose.cells.drawing.texts/textoptions/shadow/) { get; } | Represents a [`ShadowEffect`](../../aspose.cells.drawing/shadoweffect/) object that specifies shadow effect for the chart element or shape. |
| [Size](../../aspose.cells/font/size/) { get; set; } | Gets or sets the size of the font.(Inherited from [`Font`](../../aspose.cells/font/).) |
| [Spacing](../../aspose.cells.drawing.texts/textoptions/spacing/) { get; set; } | Specifies the spacing between characters within a text run. |
| [StrikeType](../../aspose.cells/font/striketype/) { get; set; } | Gets the strike type of the text.(Inherited from [`Font`](../../aspose.cells/font/).) |
| [ThemeColor](../../aspose.cells/font/themecolor/) { get; set; } | Gets and sets the theme color.(Inherited from [`Font`](../../aspose.cells/font/).) |
| [Underline](../../aspose.cells/font/underline/) { get; set; } | Gets or sets the font underline type.(Inherited from [`Font`](../../aspose.cells/font/).) |
| [UnderlineColor](../../aspose.cells.drawing.texts/textoptions/underlinecolor/) { get; set; } | Gets or sets the color of underline. |

## Methods

| Name | Description |
| --- | --- |
| [Equals](../../aspose.cells/font/equals/)(Font) | Checks if two fonts are equals.(Inherited from [`Font`](../../aspose.cells/font/).) |
| [SetName](../../aspose.cells/font/setname/)(string, FontSchemeType) | Sets name and scheme of the font.(Inherited from [`Font`](../../aspose.cells/font/).) |
| override [ToString](../../aspose.cells/font/tostring/)() | Returns a string represents the current Cell object.(Inherited from [`Font`](../../aspose.cells/font/).) |

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassTextOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add a shape to the worksheet with all required parameters
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
            
            // Add text to the shape and get TextOptions
            shape.TextBody.Text = "Sample Text";
            TextOptions textOptions = shape.TextBody[2].TextOptions;
            
            // Set text options
            textOptions.Fill.SolidFill.Color = System.Drawing.Color.Red;
            textOptions.Fill.SolidFill.Transparency = 0.5;
            
            // Save the workbook
            workbook.Save("TextOptionsDemo.xlsx");
        }
    }
}
```

### See Also

* class [Font](../../aspose.cells/font/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


