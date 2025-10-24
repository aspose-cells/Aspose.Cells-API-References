##Workbook.SetDigitalSignature
Workbook method. Sets digital signature to an spreadsheet file Excel2007 and later
## Workbook.SetDigitalSignature method
Sets digital signature to an spreadsheet file (Excel2007 and later).
```csharp
public void SetDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```
| Parameter | Type | Description |
| --- | --- | --- |
| digitalSignatureCollection | DigitalSignatureCollection |  |
### Remarks
Only support adding Xmldsig Digital Signature
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;
namespace AsposeCellsExamples
{
public class WorkbookMethodSetDigitalSignatureWithDigitalSignatureCollectionDemo
{
public static void Run()
{
// Source directory path
string sourceDir = "SourceDirectory/";
// Output directory path
string outputDir = "OutputDirectory/";
// Load the workbook
Workbook workbook = new Workbook(sourceDir + "TestCert.xlsx");
// Create digital signature collection
DigitalSignatureCollection digitalSignatures = new DigitalSignatureCollection();
// Load certificate file
string certPath = sourceDir + "certs\\sample.pfx";
byte[] certData = File.ReadAllBytes(certPath);
// Create digital signature
DigitalSignature signature = new DigitalSignature(certData, "1234567890", "Sample Signer", DateTime.Now);
// Add signature to collection
digitalSignatures.Add(signature);
// Set digital signature to workbook
workbook.SetDigitalSignature(digitalSignatures);
// Save the workbook
workbook.Save(outputDir + "DigitallySignedWorkbook.xlsx");
Console.WriteLine("Digital signature set successfully.");
}
}
}
```
### See Also
* class [DigitalSignatureCollection](../../../aspose.cells.digitalsignatures/digitalsignaturecollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
