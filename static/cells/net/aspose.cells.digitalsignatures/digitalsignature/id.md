##DigitalSignature.Id
DigitalSignature property. Specifies a GUID which can be crossreferenced with the GUID of the signature line stored in the document content. Default value is Empty all zeroes Guid
## DigitalSignature.Id property
Specifies a GUID which can be cross-referenced with the GUID of the signature line stored in the document content. Default value is Empty (all zeroes) Guid.
```csharp
public Guid Id { get; set; }
```
### Remarks
When set, it associates [`SignatureLine`](../../../aspose.cells.drawing/signatureline/) with corresponding [`DigitalSignature`](../).
### Examples
```csharp
using System;
using System.IO;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;
namespace AsposeCellsExamples
{
public class DigitalSignaturePropertyIdDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a digital signature with a specific ID
Guid signatureId = Guid.NewGuid();
// Create a digital signature
X509Certificate2 certificate = new X509Certificate2("test.pfx", "password");
DigitalSignature signature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);
// Set the signature's Id
signature.Id = signatureId;
// Add signature to collection
DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
dsCollection.Add(signature);
// Apply digital signature to workbook
workbook.SetDigitalSignature(dsCollection);
// Save the workbook
workbook.Save("signed_workbook.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)
