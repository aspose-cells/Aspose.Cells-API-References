---
title: Class SignatureLine
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.SignatureLine class. Represent the signature line
type: docs
url: /net/aspose.cells.drawing/signatureline/
---
## SignatureLine class

Represent the signature line.

```csharp
public class SignatureLine
```

## Constructors

| Name | Description |
| --- | --- |
| [SignatureLine](signatureline/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [AllowComments](../../aspose.cells.drawing/signatureline/allowcomments/) { get; set; } | Indicates whether comments could be attached. |
| [Email](../../aspose.cells.drawing/signatureline/email/) { get; set; } | Gets and sets the email of singer. |
| [Id](../../aspose.cells.drawing/signatureline/id/) { get; set; } | Gets or sets identifier for this signature line. |
| [Instructions](../../aspose.cells.drawing/signatureline/instructions/) { get; set; } | Gets and sets the text shown to user at signing time. |
| [IsLine](../../aspose.cells.drawing/signatureline/isline/) { get; set; } | Indicates whether it is a signature line. |
| [ProviderId](../../aspose.cells.drawing/signatureline/providerid/) { get; set; } | Gets and sets the id of signature provider. |
| [ShowSignedDate](../../aspose.cells.drawing/signatureline/showsigneddate/) { get; set; } | Indicates whether show signed date. |
| [Signer](../../aspose.cells.drawing/signatureline/signer/) { get; set; } | Gets and sets the signer. |
| [Title](../../aspose.cells.drawing/signatureline/title/) { get; set; } | Gets and sets the title of singer. |

### Examples

```csharp

[C#]

//Instantiating a Workbook object
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];

//Adding a picture
int imgIndex = worksheet.Pictures.Add(1, 1, "sample.png");
Picture pic = worksheet.Pictures[imgIndex];
// Create signature line object
SignatureLine s = new SignatureLine();
s.Signer = "Simon Zhao";
s.Title = "Development Lead";
s.Email = "Simon.Zhao@aspose.com";
// Assign the signature line object to Picture.SignatureLine property
pic.SignatureLine = s;

//do your business

//Save the excel file.
workbook.Save("result.xlsx");
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


