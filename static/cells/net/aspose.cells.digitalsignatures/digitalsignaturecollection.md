##Class DigitalSignatureCollection
Aspose.Cells.DigitalSignatures.DigitalSignatureCollection class. Provides a collection of digital signatures attached to a document
## DigitalSignatureCollection class
Provides a collection of digital signatures attached to a document.
```csharp
public class DigitalSignatureCollection : IEnumerable
```
## Constructors
| Name | Description |
| --- | --- |
| [DigitalSignatureCollection](digitalsignaturecollection/)() | The constructor of DigitalSignatureCollection. |
## Methods
| Name | Description |
| --- | --- |
| [Add](../../aspose.cells.digitalsignatures/digitalsignaturecollection/add/)(DigitalSignature) | Add one signature to DigitalSignatureCollection. |
| [GetEnumerator](../../aspose.cells.digitalsignatures/digitalsignaturecollection/getenumerator/)() | Get the enumerator for DigitalSignatureCollection, this enumerator allows iteration over the collection |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;
using System;
using System.Security.Cryptography.X509Certificates;
public class DigitalSignatureCollectionDemo
{
public static void DigitalSignatureCollectionExample()
{
// Load a workbook from a signed source file
Workbook signedWorkbook = new Workbook(@"DigitalSignatureCollection_original.xlsx");
// Check if the workbook is digitally signed
Console.WriteLine("Is the workbook digitally signed? " + signedWorkbook.IsDigitallySigned);
// Get the digital signature collection from the workbook
DigitalSignatureCollection existingDsc = signedWorkbook.GetDigitalSignature();
if (existingDsc != null)
{
// Iterate over the digital signatures in the collection
foreach (DigitalSignature existingDs in existingDsc)
{
Console.WriteLine("Comments: " + existingDs.Comments);
Console.WriteLine("Sign Time: " + existingDs.SignTime);
Console.WriteLine("Is Valid: " + existingDs.IsValid);
}
// Create a new digital signature
X509Certificate2 certificate = new X509Certificate2("path_to_certificate.pfx", "password");
DigitalSignature newSignature = new DigitalSignature(certificate, "New signature comment", DateTime.Now);
// Add the new digital signature to the collection
existingDsc.Add(newSignature);
}
// Save the workbook with the new digital signature
signedWorkbook.Save("DigitalSignatureCollectionExample.xlsx");
signedWorkbook.Save("DigitalSignatureCollectionExample.pdf");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells.DigitalSignatures](../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../)
