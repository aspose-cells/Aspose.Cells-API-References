##DigitalSignature.Certificate
DigitalSignature property. Certificate object that was used to sign the document
## DigitalSignature.Certificate property
Certificate object that was used to sign the document.
```csharp
public X509Certificate2 Certificate { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;
using System;
using System.Security.Cryptography.X509Certificates;
public class DigitalSignaturePropertyCertificateDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Create a certificate (in real scenario, you would load an actual certificate)
// This is just for demonstration - will not be valid for actual signing
X509Certificate2 certificate = new X509Certificate2();
// Create a digital signature with the certificate
DigitalSignature signature = new DigitalSignature(
certificate,
"Test signature",
DateTime.Now);
// Display current certificate information
Console.WriteLine("Current Certificate Subject: " + signature.Certificate.Subject);
Console.WriteLine("Current Certificate Issuer: " + signature.Certificate.Issuer);
// Create a collection and add the signature to it
DigitalSignatureCollection signatureCollection = new DigitalSignatureCollection();
signatureCollection.Add(signature);
// Add the signatures to the workbook
workbook.AddDigitalSignature(signatureCollection);
// Create a new certificate (simulated)
X509Certificate2 newCertificate = new X509Certificate2();
// Change the certificate property
signature.Certificate = newCertificate;
// Display new certificate information
Console.WriteLine("New Certificate Subject: " + signature.Certificate.Subject);
Console.WriteLine("New Certificate Issuer: " + signature.Certificate.Issuer);
// Save the workbook with digital signature
workbook.Save("DigitalSignatureWithCertificate.xlsx");
}
}
}
```
### See Also
* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)
