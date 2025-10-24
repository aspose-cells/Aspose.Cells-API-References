##DigitalSignature.Comments
DigitalSignature property. The purpose to signature
## DigitalSignature.Comments property
The purpose to signature.
```csharp
public string Comments { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;
namespace AsposeCellsExamples
{
public class DigitalSignaturePropertyCommentsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add some sample data
workbook.Worksheets[0].Cells["A1"].PutValue("Test Digital Signature with Comments");
// Create digital signature with comments
DigitalSignature signature = new DigitalSignature(
File.ReadAllBytes("sample.pfx"),
"password",
"Sample Signature with Comments",
DateTime.Now)
{
Comments = "This is a test comment for the digital signature"
};
// Add signature to collection
DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
dsCollection.Add(signature);
// Sign the workbook
workbook.SetDigitalSignature(dsCollection);
// Save the signed workbook
string outputPath = "SignedWithComments.xlsx";
workbook.Save(outputPath);
// Verify and display signature info
Workbook signedWorkbook = new Workbook(outputPath);
DigitalSignatureCollection signatures = signedWorkbook.GetDigitalSignature();
foreach (DigitalSignature ds in signatures)
{
Console.WriteLine($"Comments: {ds.Comments}");
Console.WriteLine($"Sign Time: {ds.SignTime}");
Console.WriteLine($"Is Valid: {ds.IsValid}");
}
}
}
}
```
### See Also
* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)
