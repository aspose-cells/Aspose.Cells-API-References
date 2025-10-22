##DigitalSignature.DigitalSignature
DigitalSignature constructor. Constructor of digitalSignature. Uses .Net implementation
## DigitalSignature(X509Certificate2, string, DateTime) {#constructor_1}
Constructor of digitalSignature. Uses .Net implementation.
```csharp
public DigitalSignature(X509Certificate2 certificate, string comments, DateTime signTime)
```
| Parameter | Type | Description |
| --- | --- | --- |
| certificate | X509Certificate2 | Certificate object that was used to sign the document. |
| comments | String | The purpose to signature. |
| signTime | DateTime | The utc time when the document was signed. |
### Examples
```csharp
using System;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;
namespace AsposeCellsExamples
{
public class DigitalSignatureMethodCtorWithX509Certificate2StringDateTimeDemo
{
public static void Run()
{
// Create a digital signature collection
DigitalSignatureCollection signatures = new DigitalSignatureCollection();
// Load certificate with private key
X509Certificate2 certificate = new X509Certificate2("mykey2.pfx", "123456");
// Create digital signature with certificate, purpose and timestamp
DigitalSignature signature = new DigitalSignature(
certificate,
"Document approval",
DateTime.Now);
signatures.Add(signature);
// Create a new workbook and sign it
Workbook workbook = new Workbook();
workbook.SetDigitalSignature(signatures);
workbook.Save("signed_document.xlsx");
}
}
}
```
### See Also
* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)
## DigitalSignature(byte[], string, string, DateTime) {#constructor}
Constructor of digitalSignature. Uses Bouncy Castle implementation.
```csharp
public DigitalSignature(byte[] rawData, string password, string comments, DateTime signTime)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rawData | Byte[] | A byte array containing data from an X.509 certificate. |
| password | String | The password required to access the X.509 certificate data. |
| comments | String | The purpose to signature. |
| signTime | DateTime | The utc time when the document was signed. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;
using System;
using System.IO;
public class DigitalSignatureConstructorWithByteArrayStringStringDateTimeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample content
worksheet.Cells["A1"].PutValue("Digitally Signed Document");
try
{
// Load certificate file as byte array (replace with actual certificate path)
string certPath = "certificate.pfx";
byte[] certData = File.ReadAllBytes(certPath);
// Create digital signature parameters
string password = "certificate_password";
string comments = "Approved by John Doe";
DateTime signTime = DateTime.Now;
// Call the constructor with (Byte[], String, String, DateTime)
DigitalSignature signature = new DigitalSignature(certData, password, comments, signTime);
// Create a DigitalSignatureCollection and add the signature to it
DigitalSignatureCollection signatures = new DigitalSignatureCollection();
signatures.Add(signature);
// Add signatures to workbook
workbook.AddDigitalSignature(signatures);
Console.WriteLine("Digital signature added successfully with parameters (Byte[], String, String, DateTime)");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing constructor method: {ex.Message}");
}
// Save the result
workbook.Save("DigitalSignatureDemo.xlsx");
}
}
}
```
### See Also
* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)
