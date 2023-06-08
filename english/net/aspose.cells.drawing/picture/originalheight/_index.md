---
title: Picture.OriginalHeight
second_title: Aspose.Cells for .NET API Reference
description: Picture property. Gets the original height of the picture
type: docs
url: /net/aspose.cells.drawing/picture/originalheight/
---
## Picture.OriginalHeight property

Gets the original height of the picture.

```csharp
public int OriginalHeight { get; }
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
//Gets the original height of the picture.
int picHeight = pic.OriginalHeight;
//Save the excel file.
workbook.Save("result.xlsx");
```

### See Also

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


