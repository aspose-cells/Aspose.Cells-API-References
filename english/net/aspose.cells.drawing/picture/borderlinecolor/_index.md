---
title: Picture.BorderLineColor
second_title: Aspose.Cells for .NET API Reference
description: Picture property. Represents the Color of the border line of a picture
type: docs
url: /net/aspose.cells.drawing/picture/borderlinecolor/
---
## Picture.BorderLineColor property

Represents the Color of the border line of a picture.

```csharp
public Color BorderLineColor { get; set; }
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
//Set the border color of the picture
pic.BorderLineColor = Color.Red;
//Save the excel file.
workbook.Save("result.xlsx");
```

### See Also

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


