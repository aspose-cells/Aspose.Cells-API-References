##Workbook.RemoveDigitalSignature
Workbook method. Removes digital signature from this spreadsheet
## Workbook.RemoveDigitalSignature method
Removes digital signature from this spreadsheet.
```csharp
public void RemoveDigitalSignature()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodRemoveDigitalSignatureDemo
{
public static void Run()
{
// Create a workbook with digital signature
Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
sheet.Cells["A1"].PutValue("Test Digital Signature");
// Save with digital signature (in real scenario this would be signed externally)
string signedPath = "SignedWorkbook.xlsx";
book.Save(signedPath, SaveFormat.Xlsx);
// Load the signed workbook
Workbook signedBook = new Workbook(signedPath);
Console.WriteLine("Workbook is digitally signed: " + signedBook.IsDigitallySigned);
// Remove digital signature
signedBook.RemoveDigitalSignature();
string unsignedPath = "UnsignedWorkbook.xlsx";
signedBook.Save(unsignedPath);
// Verify signature was removed
Workbook unsignedBook = new Workbook(unsignedPath);
Console.WriteLine("After removal, workbook is digitally signed: " + unsignedBook.IsDigitallySigned);
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
