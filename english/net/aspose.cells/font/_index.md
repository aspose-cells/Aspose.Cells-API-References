---
title: Class Font
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Font class. Encapsulates the font object used in a spreadsheet
type: docs
url: /net/aspose.cells/font/
---
## Font class

Encapsulates the font object used in a spreadsheet.

```csharp
public class Font
```

## Properties

| Name | Description |
| --- | --- |
| [ArgbColor](../../aspose.cells/font/argbcolor/) { get; set; } | Gets and sets the color with a 32-bit ARGB value. |
| [CapsType](../../aspose.cells/font/capstype/) { get; set; } | Gets and sets the text caps type. |
| [Charset](../../aspose.cells/font/charset/) { get; set; } | Represent the character set. |
| [Color](../../aspose.cells/font/color/) { get; set; } | Gets or sets the Color of the font. |
| [DoubleSize](../../aspose.cells/font/doublesize/) { get; set; } | Gets and sets the double size of the font. |
| [IsBold](../../aspose.cells/font/isbold/) { get; set; } | Gets or sets a value indicating whether the font is bold. |
| [IsItalic](../../aspose.cells/font/isitalic/) { get; set; } | Gets or sets a value indicating whether the font is italic. |
| [IsNormalizeHeights](../../aspose.cells/font/isnormalizeheights/) { get; set; } | Indicates whether the normalization of height that is to be applied to the text run. |
| [IsStrikeout](../../aspose.cells/font/isstrikeout/) { get; set; } | Gets or sets a value indicating whether the font is single strikeout. |
| [IsSubscript](../../aspose.cells/font/issubscript/) { get; set; } | Gets or sets a value indicating whether the font is subscript. |
| [IsSuperscript](../../aspose.cells/font/issuperscript/) { get; set; } | Gets or sets a value indicating whether the font is super script. |
| virtual [Name](../../aspose.cells/font/name/) { get; set; } | Gets or sets the name of the `Font`. |
| [SchemeType](../../aspose.cells/font/schemetype/) { get; set; } | Gets and sets the scheme type of the font. |
| [ScriptOffset](../../aspose.cells/font/scriptoffset/) { get; set; } | Gets and sets the script offset,in unit of percentage |
| [Size](../../aspose.cells/font/size/) { get; set; } | Gets or sets the size of the font. |
| [StrikeType](../../aspose.cells/font/striketype/) { get; set; } | Gets the strike type of the text. |
| [ThemeColor](../../aspose.cells/font/themecolor/) { get; set; } | Gets and sets the theme color. |
| [Underline](../../aspose.cells/font/underline/) { get; set; } | Gets or sets the font underline type. |

## Methods

| Name | Description |
| --- | --- |
| [Equals](../../aspose.cells/font/equals/#equals)(Font) | Checks if two fonts are equals. |
| override [ToString](../../aspose.cells/font/tostring/)() | Returns a string represents the current Cell object. |

### Examples

```csharp

[C#]

//Instantiating a Workbook object
Workbook workbook = new Workbook();

//Obtaining the reference of the newly added worksheet by passing its sheet index
Worksheet worksheet = workbook.Worksheets[0];

//Accessing the "A1" cell from the worksheet
Aspose.Cells.Cell cell = worksheet.Cells["A1"];

//Adding some value to the "A1" cell
cell.PutValue("Hello Aspose!");

Aspose.Cells.Font font = cell.GetStyle().Font;

//Setting the font name to "Times New Roman"
font.Name = "Times New Roman";

//Setting font size to 14
font.Size = 14;

//setting font color as Red
font.Color = System.Drawing.Color.Red;           

//Saving the Excel file
workbook.Save(@"dest.xls");

[VB.NET]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()

'Obtaining the reference of the newly added worksheet by passing its sheet index
Dim worksheet As Worksheet = workbook.Worksheets(0)

'Accessing the "A1" cell from the worksheet
Dim cell As Aspose.Cells.Cell = worksheet.Cells("A1")

'Adding some value to the "A1" cell
cell.PutValue("Hello Aspose!")

Dim font As Aspose.Cells.Font = cell.GetStyle().Font

'Setting the font name to "Times New Roman"
font.Name = "Times New Roman"

'Setting font size to 14
font.Size = 14

'setting font color as Red
font.Color = System.Drawing.Color.Red

'Saving the Excel file
workbook.Save("dest.xls")
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


