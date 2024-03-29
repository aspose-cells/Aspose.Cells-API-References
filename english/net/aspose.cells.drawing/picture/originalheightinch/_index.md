---
title: Picture.OriginalHeightInch
second_title: Aspose.Cells for .NET API Reference
description: Picture property. Gets the original height of picture in unit of inches
type: docs
url: /net/aspose.cells.drawing/picture/originalheightinch/
---
## Picture.OriginalHeightInch property

Gets the original height of picture, in unit of inches.

```csharp
public double OriginalHeightInch { get; }
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
double picHeightInch = pic.OriginalHeightInch;
//Save the excel file.
workbook.Save("result.xlsx");
```

### See Also

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


