---
title: Picture.SignatureLine
second_title: Aspose.Cells for .NET API Reference
description: Picture property. Gets and sets the signature line
type: docs
url: /net/aspose.cells.drawing/picture/signatureline/
---
## Picture.SignatureLine property

Gets and sets the signature line

```csharp
public SignatureLine SignatureLine { get; set; }
```

### Examples

```csharp

[C#]
//Instantiating a Workbook object
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
//Adding a picture at the location of a cell whose row and column indices are 1 in the worksheet. It is "B2" cell
int imgIndex = worksheet.Pictures.Add(1, 1, (string)null);
//Get the inserted picture object
Picture pic = worksheet.Pictures[imgIndex];
// Create signature line object
SignatureLine s = new SignatureLine();
s.Signer = "Simon";
s.Title = "Development";
s.Email = "simon@aspose.com";
// Assign the signature line object to Picture.
pic.SignatureLine = s;
//Save the excel file.
workbook.Save("result.xlsx");
```

### See Also

* class [SignatureLine](../../signatureline/)
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


