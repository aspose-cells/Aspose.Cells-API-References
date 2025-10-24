##DigitalSignature.Image
DigitalSignature property. Specifies an image for the digital signature. Default value is null
## DigitalSignature.Image property
Specifies an image for the digital signature. Default value is null.
```csharp
public byte[] Image { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.DigitalSignatures;
using System.Security.Cryptography.X509Certificates;
namespace AsposeCellsExamples
{
public class DigitalSignaturePropertyImageDemo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
Worksheet ws = wb.Worksheets[0];
// Add a signature line to the worksheet
Picture picture = ws.Pictures[0];
SignatureLine signatureLine = picture.SignatureLine;
signatureLine.Signer = "Test Signer";
signatureLine.Title = "Test Title";
// Create a test certificate (in real usage, load from file)
byte[] certData = new byte[0]; // Replace with actual certificate bytes
X509Certificate2 certificate = new X509Certificate2(certData);
// Create digital signature with image
DigitalSignature signature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);
signature.Image = File.ReadAllBytes("signature.png"); // Replace with actual image path
// Add signature and save
DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
dsCollection.Add(signature);
wb.SetDigitalSignature(dsCollection);
// Save to memory stream
MemoryStream ms = new MemoryStream();
wb.Save(ms, SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)
