---
title: Picture.BorderWeight
second_title: Aspose.Cells for .NET API Reference
description: Picture property. Gets or sets the weight of the border line of a picture in units of pt
type: docs
url: /net/aspose.cells.drawing/picture/borderweight/
---
## Picture.BorderWeight property

Gets or sets the weight of the border line of a picture in units of pt.

```csharp
public double BorderWeight { get; set; }
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
//Set the border width of the picture
pic.BorderWeight = 3;
//Save the excel file.
workbook.Save("result.xlsx");
```

### See Also

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


