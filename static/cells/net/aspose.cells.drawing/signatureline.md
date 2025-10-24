##Class SignatureLine
Aspose.Cells.Drawing.SignatureLine class. Represent the signature line
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
| [Email](../../aspose.cells.drawing/signatureline/email/) { get; set; } | Gets or sets the email of singer. |
| [Id](../../aspose.cells.drawing/signatureline/id/) { get; set; } | Gets or sets identifier for this signature line. |
| [Instructions](../../aspose.cells.drawing/signatureline/instructions/) { get; set; } | Gets or sets the text shown to user at signing time. |
| [IsLine](../../aspose.cells.drawing/signatureline/isline/) { get; set; } | Indicates whether it is a signature line. |
| [ProviderId](../../aspose.cells.drawing/signatureline/providerid/) { get; set; } | Gets or sets the id of signature provider. |
| [ShowSignedDate](../../aspose.cells.drawing/signatureline/showsigneddate/) { get; set; } | Indicates whether show signed date. |
| [SignatureLineType](../../aspose.cells.drawing/signatureline/signaturelinetype/) { get; set; } | Gets or sets the signature type. Default - When the default value is set, the corresponding ProviderId value is fixed to {0000000000-0000-0000-0000-0000000000}. Stamp - When the value is Stamp, the corresponding ProviderId value is usually {000CD6A4-0000-0000-C000-000000000046}. Custom - When the value is Custom, the corresponding ProviderId value usually needs to be set by the user. it should be obtained from the documentation shipped with the provider. |
| [Signer](../../aspose.cells.drawing/signatureline/signer/) { get; set; } | Gets or sets the signer. |
| [Title](../../aspose.cells.drawing/signatureline/title/) { get; set; } | Gets or sets the title of singer. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class SignatureLineDemo
{
public static void SignatureLineExample()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Adding a picture
int imgIndex = worksheet.Pictures.Add(1, 1, "SignatureLineExample_original.png");
Picture pic = worksheet.Pictures[imgIndex];
// Create signature line object
SignatureLine s = new SignatureLine();
s.Signer = "Simon Zhao";
s.Title = "Development Lead";
s.Email = "Simon.Zhao@aspose.com";
s.Id = Guid.NewGuid();
s.ProviderId = Guid.NewGuid();
s.IsLine = true;
s.AllowComments = true;
s.ShowSignedDate = true;
s.Instructions = "Just do it.";
// Assign the signature line object to Picture.SignatureLine property
pic.SignatureLine = s;
// Save the excel file
workbook.Save("SignatureLineExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
