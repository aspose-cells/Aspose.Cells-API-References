---
title: Class FontSetting
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.FontSetting class. Represents a range of characters within the cell text
type: docs
url: /net/aspose.cells/fontsetting/
---
## FontSetting class

Represents a range of characters within the cell text.

```csharp
public class FontSetting
```

## Constructors

| Name | Description |
| --- | --- |
| [FontSetting](fontsetting/)(int, int, WorksheetCollection) |  |

## Properties

| Name | Description |
| --- | --- |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Returns the font of this object. |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Gets the length of the characters. |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Gets the start index of the characters. |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Returns the text options. |
| virtual [Type](../../aspose.cells/fontsetting/type/) { get; } | Gets the type of text node. |

## Methods

| Name | Description |
| --- | --- |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Sets the preset WordArt style. |

### Examples

```csharp

[C#]

//Instantiating a Workbook object
Workbook workbook = new Workbook();

//Adding a new worksheet to the Excel object
workbook.Worksheets.Add();

//Obtaining the reference of the newly added worksheet by passing its sheet index
Worksheet worksheet = workbook.Worksheets[0];

//Accessing the "A1" cell from the worksheet
Aspose.Cells.Cell cell = worksheet.Cells["A1"];

//Adding some value to the "A1" cell
cell.PutValue("Visit Aspose!");

//getting charactor
FontSetting charactor = cell.Characters(6, 7);

//Setting the font of selected characters to bold
charactor.Font.IsBold = true;

//Setting the font color of selected characters to blue
charactor.Font.Color = Color.Blue;

//Saving the Excel file
workbook.Save("book1.xls");

[VB.NET]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()

'Adding a new worksheet to the Excel object
workbook.Worksheets.Add()

'Obtaining the reference of the newly added worksheet by passing its sheet index
Dim worksheet As Worksheet = workbook.Worksheets(0)

'Accessing the "A1" cell from the worksheet
Dim cell As Aspose.Cells.Cell = worksheet.Cells("A1")

'Adding some value to the "A1" cell
cell.PutValue("Visit Aspose!")

'getting charactor
Dim charactor As FontSetting = cell.Characters(6, 7)

'Setting the font of selected characters to bold
charactor.Font.IsBold = True

'Setting the font color of selected characters to blue
charactor.Font.Color = Color.Blue

'Saving the Excel file
workbook.Save("book1.xls")
 
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


