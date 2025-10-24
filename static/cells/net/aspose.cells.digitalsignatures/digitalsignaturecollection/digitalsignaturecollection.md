##DigitalSignatureCollection.DigitalSignatureCollection
DigitalSignatureCollection constructor. The constructor of DigitalSignatureCollection
## DigitalSignatureCollection constructor
The constructor of DigitalSignatureCollection.
```csharp
public DigitalSignatureCollection()
```
### Examples
```csharp
using System;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;
namespace AsposeCellsExamples
{
public class DigitalSignatureCollectionMethodCtorDemo
{
public static void Run()
{
// Initialize a new DigitalSignatureCollection
DigitalSignatureCollection certSigns = new DigitalSignatureCollection();
// Load certificate and create digital signature
string pfx = "ForTest.pfx";
string password = "123456";
string comment = "test";
X509Certificate2 cert = new X509Certificate2(pfx, password);
DigitalSignature certSign = new DigitalSignature(cert, comment, DateTime.Now);
// Add signature to collection
certSigns.Add(certSign);
Console.WriteLine("Digital signature collection created with 1 signature.");
}
}
}
```
### See Also
* class [DigitalSignatureCollection](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)
