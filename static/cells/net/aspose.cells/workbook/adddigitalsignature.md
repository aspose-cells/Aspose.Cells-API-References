##Workbook.AddDigitalSignature
Workbook method. Adds digital signature to an OOXML spreadsheet file Excel2007 and later
## Workbook.AddDigitalSignature method
Adds digital signature to an OOXML spreadsheet file (Excel2007 and later).
```csharp
public void AddDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```
| Parameter | Type | Description |
| --- | --- | --- |
| digitalSignatureCollection | DigitalSignatureCollection |  |
### Remarks
Only support adding Xmldsig Digital Signature to an OOXML spreadsheet file
### Examples
```csharp
using System;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;
namespace AsposeCellsExamples
{
public class WorkbookMethodAddDigitalSignatureWithDigitalSignatureCollectionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add some sample data
workbook.Worksheets[0].Cells["A1"].PutValue("Test Digital Signature");
// Load certificate (replace with your own certificate path and password)
X509Certificate2 certificate = new X509Certificate2("DrWatson.pfx", "1234567890");
// Create digital signature
DigitalSignature digitalSignature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);
// Create digital signature collection and add signature
DigitalSignatureCollection digitalSignatureCollection = new DigitalSignatureCollection();
digitalSignatureCollection.Add(digitalSignature);
// Add digital signature to workbook
workbook.AddDigitalSignature(digitalSignatureCollection);
// Save the workbook
workbook.Save("DigitallySignedWorkbook.xlsx");
}
}
}
```
### See Also
* class [DigitalSignatureCollection](../../../aspose.cells.digitalsignatures/digitalsignaturecollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
