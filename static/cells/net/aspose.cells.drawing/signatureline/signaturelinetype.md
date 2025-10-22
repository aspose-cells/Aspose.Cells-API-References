##SignatureLine.SignatureLineType
SignatureLine property. Gets or sets the signature type. Default  When the default value is set the corresponding ProviderId value is fixed to 00000000000000000000000000000000. Stamp  When the value is Stamp the corresponding ProviderId value is usually 000CD6A400000000C000000000000046. Custom  When the value is Custom the corresponding ProviderId value usually needs to be set by the user. it should be obtained from the documentation shipped with the provider
## SignatureLine.SignatureLineType property
Gets or sets the signature type. Default - When the default value is set, the corresponding ProviderId value is fixed to {0000000000-0000-0000-0000-0000000000}. Stamp - When the value is Stamp, the corresponding ProviderId value is usually {000CD6A4-0000-0000-C000-000000000046}. Custom - When the value is Custom, the corresponding ProviderId value usually needs to be set by the user. it should be obtained from the documentation shipped with the provider.
```csharp
public SignatureType SignatureLineType { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class SignatureLinePropertySignatureLineTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a signature line
SignatureLine signatureLine = new SignatureLine();
signatureLine.Signer = "John Doe";
signatureLine.Title = "Developer";
signatureLine.Email = "john@example.com";
signatureLine.IsLine = true;
signatureLine.AllowComments = true;
signatureLine.ShowSignedDate = true;
signatureLine.Instructions = "Please sign here";
// Display current SignatureLineType
Console.WriteLine("Current SignatureLineType: " + signatureLine.SignatureLineType);
// Set SignatureLineType to Stamp
signatureLine.SignatureLineType = SignatureType.Stamp;
Console.WriteLine("Changed SignatureLineType to: " + signatureLine.SignatureLineType);
Console.WriteLine("ProviderId after Stamp type: " + signatureLine.ProviderId);
// Add the signature line to the worksheet by adding it to shapes
Picture signaturePicture = worksheet.Shapes.AddSignatureLine(0, 0, signatureLine); // Changed to Picture type
Console.WriteLine("Added signature line with index: " + signaturePicture.OriginalHeight);
// Change SignatureLineType to Custom with custom ProviderId
signatureLine.SignatureLineType = SignatureType.Custom;
signatureLine.ProviderId = Guid.NewGuid();
Console.WriteLine("Changed SignatureLineType to: " + signatureLine.SignatureLineType);
Console.WriteLine("Custom ProviderId: " + signatureLine.ProviderId);
// Save the workbook
workbook.Save("SignatureLineTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [SignatureType](../../signaturetype/)
* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
