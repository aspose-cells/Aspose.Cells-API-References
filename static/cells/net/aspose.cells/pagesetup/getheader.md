##PageSetup.GetHeader
PageSetup method. Gets a script formatting the header of an Excel file
## PageSetup.GetHeader method
Gets a script formatting the header of an Excel file.
```csharp
public string GetHeader(int section)
```
| Parameter | Type | Description |
| --- | --- | --- |
| section | Int32 | 0: Left Section, 1: Center Section, 2: Right Section. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupMethodGetHeaderWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set header for section 2
worksheet.PageSetup.SetHeader(2, "&8Report ID: TEST01\n你好Public");
// Get and print the header for section 2
string header = worksheet.PageSetup.GetHeader(2);
Console.WriteLine("Header for section 2: " + header);
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
