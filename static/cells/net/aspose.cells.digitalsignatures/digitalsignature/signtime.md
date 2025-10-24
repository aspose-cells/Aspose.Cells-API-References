##DigitalSignature.SignTime
DigitalSignature property. The time when the document was signed
## DigitalSignature.SignTime property
The time when the document was signed.
```csharp
public DateTime SignTime { get; set; }
```
### Examples
```csharp
using System;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;
namespace AsposeCellsExamples
{
public class DigitalSignaturePropertySignTimeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Test Digital Signature");
// Create and add a digital signature
try
{
X509Certificate2 certificate = new X509Certificate2("test.pfx", "password");
DigitalSignature signature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);
DigitalSignatureCollection dsc = workbook.GetDigitalSignature();
dsc.Add(signature);
// Demonstrate SignTime property
Console.WriteLine("Signature added at: " + signature.SignTime);
// Save the signed workbook
workbook.Save("SignedWorkbook.xlsx");
}
catch (Exception ex)
{
Console.WriteLine("Error: " + ex.Message);
}
}
}
}
```
### See Also
* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)
