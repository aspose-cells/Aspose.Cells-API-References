##SignatureLine.ProviderId
SignatureLine property. Gets or sets the id of signature provider
## SignatureLine.ProviderId property
Gets or sets the id of signature provider.
```csharp
public Guid ProviderId { get; set; }
```
### Remarks
It's typically the CLSID of the provider com add-in.
### Examples
```csharp
using System;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class SignatureLinePropertyProviderIdDemo
{
public static void Run()
{
// Create a new signature line
SignatureLine signatureLine = new SignatureLine();
// Set signature line properties
signatureLine.Signer = "John Doe";
signatureLine.Title = "Software Developer";
signatureLine.Email = "john.doe@example.com";
signatureLine.IsLine = true;
// Set provider ID (example GUID - should be replaced with actual provider GUID)
signatureLine.ProviderId = new Guid("000CD6A4-0000-0000-C000-000000000046");
// Set signature type (this should match the provider ID)
signatureLine.SignatureLineType = SignatureType.Stamp;
// Output the provider ID to demonstrate usage
Console.WriteLine("Signature Line Provider ID: " + signatureLine.ProviderId);
}
}
}
```
### See Also
* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
