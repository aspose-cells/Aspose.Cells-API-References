##Workbook.IsDigitallySigned
Workbook property. Indicates if this spreadsheet is digitally signed
## Workbook.IsDigitallySigned property
Indicates if this spreadsheet is digitally signed.
```csharp
public bool IsDigitallySigned { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookPropertyIsDigitallySignedDemo
{
public static void Run()
{
// Load a digitally signed workbook
Workbook book = new Workbook("Test_DigiSign.xlsx");
// Check if the workbook is digitally signed
bool isSigned = book.IsDigitallySigned;
Console.WriteLine("Workbook is digitally signed: " + isSigned);
if (isSigned)
{
// Save a copy (signature will be preserved)
book.Save("SignedCopy.xlsx");
// Remove the digital signature
book.RemoveDigitalSignature();
book.Save("UnsignedCopy.xlsx");
// Verify signature was removed
Workbook unsignedBook = new Workbook("UnsignedCopy.xlsx");
Console.WriteLine("After removal, workbook is signed: " + unsignedBook.IsDigitallySigned);
}
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
