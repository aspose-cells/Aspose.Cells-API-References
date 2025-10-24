##Worksheet.AllowEditRanges
Worksheet property. Gets the allow edit range collection in the worksheet
## Worksheet.AllowEditRanges property
Gets the allow edit range collection in the worksheet.
```csharp
public ProtectedRangeCollection AllowEditRanges { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyAllowEditRangesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an allow edit range
int index = worksheet.AllowEditRanges.Add("r1", 0, 0, 1, 1);
ProtectedRange range = worksheet.AllowEditRanges[index];
range.Password = "password123";
// Protect the worksheet
worksheet.Protect(ProtectionType.All);
// Save the workbook
workbook.Save("output.xlsx");
// Load the saved workbook to verify
Workbook verifyWorkbook = new Workbook("output.xlsx");
ProtectedRange verifyRange = verifyWorkbook.Worksheets[0].AllowEditRanges[0];
Console.WriteLine("Is protected with password: " + verifyRange.IsProtectedWithPassword);
}
}
}
```
### See Also
* class [ProtectedRangeCollection](../../protectedrangecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
