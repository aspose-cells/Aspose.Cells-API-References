---
title: Picture.Move
second_title: Aspose.Cells for .NET API Reference
description: Picture method. Moves the picture to a specified location
type: docs
url: /net/aspose.cells.drawing/picture/move/
---
## Picture.Move method

Moves the picture to a specified location.

```csharp
public void Move(int upperLeftRow, int upperLeftColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| upperLeftColumn | Int32 | Upper left column index. |

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
//Set the new location of the picture
pic.Move(2, 4);
//Save the excel file.
workbook.Save("result.xlsx");
```

### See Also

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


