##DigitalSignature.IsValid
DigitalSignature property. If this digital signature is valid and the document has not been tampered with this value will be true
## DigitalSignature.IsValid property
If this digital signature is valid and the document has not been tampered with, this value will be true.
```csharp
public bool IsValid { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;
using System.IO;
namespace AsposeCellsExamples
{
public class DigitalSignaturePropertyIsValidDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add some data to the worksheet
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Test Digital Signature");
// Save the workbook first
string outputPath = "signed_example.xlsx";
workbook.Save(outputPath, SaveFormat.Xlsx);
// Create a digital signature collection
DigitalSignatureCollection signatures = new DigitalSignatureCollection();
// Create a digital signature (in real scenario, use proper certificate)
// First parameter should be byte[] of certificate data
byte[] certificateData = File.ReadAllBytes("test.pfx");
DigitalSignature signature = new DigitalSignature(
certificateData,
"test123",
"Test Signature",
DateTime.Now);
signatures.Add(signature);
// Sign the workbook
workbook.SetDigitalSignature(signatures);
workbook.Save(outputPath, SaveFormat.Xlsx);
// Verify the signature
Workbook signedWorkbook = new Workbook(outputPath);
DigitalSignatureCollection loadedSignatures = signedWorkbook.GetDigitalSignature();
foreach (DigitalSignature sig in loadedSignatures)
{
Console.WriteLine("Signature is valid: " + sig.IsValid);
}
}
}
}
```
### See Also
* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)
