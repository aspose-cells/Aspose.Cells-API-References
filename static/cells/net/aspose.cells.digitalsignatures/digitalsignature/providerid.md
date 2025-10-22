##DigitalSignature.ProviderId
DigitalSignature property. Specifies the class ID of the signature provider. Default value is Empty all zeroes Guid
## DigitalSignature.ProviderId property
Specifies the class ID of the signature provider. Default value is Empty (all zeroes) Guid.
```csharp
public Guid ProviderId { get; set; }
```
### Remarks
The cryptographic service provider (CSP) is an independent software module that actually performs cryptography algorithms for authentication, encoding, and encryption. Microsoft Office reserves the value of {00000000-0000-0000-0000-000000000000} for its default signature provider, and {000CD6A4-0000-0000-C000-000000000046} for its East Asian signature provider. The GUID of the additionally installed provider should be obtained from the documentation shipped with the provider.
### Examples
```csharp
using System;
using System.IO;
using System.Security.Cryptography;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class DigitalSignaturePropertyProviderIdDemo
{
public static void Run()
{
// Create self-signed certificate
X509Certificate2 certificate;
using (var rsa = RSA.Create())
{
var request = new CertificateRequest(
new X500DistinguishedName("cn=AsposeTest"),
rsa,
HashAlgorithmName.SHA256,
RSASignaturePadding.Pkcs1);
certificate = request.CreateSelfSigned(DateTimeOffset.Now, DateTimeOffset.Now.AddHours(1));
}
// Create workbook and add signature line
Workbook wb = new Workbook();
Worksheet ws = wb.Worksheets[0];
// Add dummy picture with signature line
using (var ms = new MemoryStream())
{
ms.Write(new byte[] { 0x42, 0x4D, 0x1E, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x1A, 0x00, 0x00, 0x00 }, 0, 14);
ms.Position = 0;
int idx = ws.Pictures.Add(0, 0, ms);
Picture pic = ws.Pictures[idx];
pic.SignatureLine = new SignatureLine();
pic.SignatureLine.ProviderId = Guid.NewGuid();
}
// Create digital signature
var signature = new DigitalSignature(certificate, "Aspose ProviderId Demo", DateTime.Now);
signature.ProviderId = ws.Pictures[0].SignatureLine.ProviderId;
// Set digital signature and save
DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
dsCollection.Add(signature);
wb.SetDigitalSignature(dsCollection);
using (MemoryStream output = new MemoryStream())
{
wb.Save(output, SaveFormat.Xlsx);
}
}
}
}
```
### See Also
* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)
