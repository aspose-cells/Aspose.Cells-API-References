---
title: Picture.OriginalWidth
second_title: Aspose.Cells for .NET API Reference
description: Picture property. Gets the original width of the picture
type: docs
url: /net/aspose.cells.drawing/picture/originalwidth/
---
## Picture.OriginalWidth property

Gets the original width of the picture.

```csharp
public int OriginalWidth { get; }
```

### Examples

```csharp

[C#]
//Instantiating a Workbook object
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
//Adding a picture at the location of a cell whose row and column indices are 1 in the worksheet. It is "B2" cell
int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
//Get the inserted picture object
Picture pic = worksheet.Pictures[imgIndex];
//Gets the original width of the picture.
int picWidth = pic.OriginalWidth;
//Save the excel file.
workbook.Save("result.xlsx");
```

### See Also

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


