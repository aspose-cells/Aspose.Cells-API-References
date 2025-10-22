##PageSetup.SetEvenHeader
PageSetup method. Sets a script formatting the even page header of an Excel file. Only effect in Excel 2007 when IsHFDiffOddEven is true
## PageSetup.SetEvenHeader method
Sets a script formatting the even page header of an Excel file. Only effect in Excel 2007 when IsHFDiffOddEven is true.
```csharp
public void SetEvenHeader(int section, string headerScript)
```
| Parameter | Type | Description |
| --- | --- | --- |
| section | Int32 | 0: Left Section, 1: Center Section, 2: Right Section. |
| headerScript | String | Header format script. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupMethodSetEvenHeaderWithInt32StringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
PageSetup pageSetup = worksheet.PageSetup;
// Enable different headers/footers for odd and even pages
pageSetup.IsHFDiffOddEven = true;
// Set even page header with section index and text
pageSetup.SetEvenHeader(1, "Even Page Header - Center Section");
pageSetup.SetEvenHeader(0, "Even Page Header - Left Section");
pageSetup.SetEvenHeader(2, "Even Page Header - Right Section");
// Save the workbook
workbook.Save("PageSetup_SetEvenHeaderExample.xlsx");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
