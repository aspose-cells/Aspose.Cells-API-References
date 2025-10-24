##VbaProject.Sign
VbaProject method. Sign this VBA project by a DigitalSignature
## VbaProject.Sign method
Sign this VBA project by a DigitalSignature
```csharp
public void Sign(DigitalSignature digitalSignature)
```
| Parameter | Type | Description |
| --- | --- | --- |
| digitalSignature | DigitalSignature | DigitalSignature |
### Examples
```csharp
using System;
using System.IO;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.Vba;
using Aspose.Cells.DigitalSignatures;
namespace AsposeCellsExamples
{
public class VbaProjectMethodSignWithDigitalSignatureDemo
{
public static void Run()
{
// Load the workbook with VBA project
Workbook workbook = new Workbook("SignXlsm.xlsm");
// Get the VBA project
VbaProject vbaProject = workbook.VbaProject;
if (vbaProject != null)
{
// Load certificate from file
X509Certificate2 certificate = new X509Certificate2("YourCertificate.pfx", "password");
// Create a digital signature
DigitalSignature certSign = new DigitalSignature(certificate, "Test Signing", DateTime.Now);
// Sign the VBA project
vbaProject.Sign(certSign);
// Save the signed workbook
using (MemoryStream stream = new MemoryStream())
{
workbook.Save(stream, SaveFormat.Xlsm);
// Verify the signature
Workbook verifyWorkbook = new Workbook(stream);
Console.WriteLine("Is Signed: " + verifyWorkbook.VbaProject.IsSigned);
Console.WriteLine("Is Valid Signed: " + verifyWorkbook.VbaProject.IsValidSigned);
}
}
}
}
}
```
### See Also
* class [DigitalSignature](../../../aspose.cells.digitalsignatures/digitalsignature/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
