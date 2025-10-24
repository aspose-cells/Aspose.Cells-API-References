##SignatureLine.Email
SignatureLine property. Gets or sets the email of singer
## SignatureLine.Email property
Gets or sets the email of singer.
```csharp
public string Email { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class SignatureLinePropertyEmailDemo
{
public static void Run()
{
// Create a new signature line
SignatureLine signatureLine = new SignatureLine();
// Set signature line properties including Email
signatureLine.Signer = "Simon Zhao";
signatureLine.Title = "Software Developer";
signatureLine.Email = "Simon.Zhao@aspose.com";
signatureLine.IsLine = true;
signatureLine.ShowSignedDate = true;
// Display the email property
Console.WriteLine("Signer Email: " + signatureLine.Email);
}
}
}
```
### See Also
* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
