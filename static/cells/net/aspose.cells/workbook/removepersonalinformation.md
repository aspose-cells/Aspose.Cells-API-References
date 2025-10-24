##Workbook.RemovePersonalInformation
Workbook method. Removes personal information
## Workbook.RemovePersonalInformation method
Removes personal information.
```csharp
public void RemovePersonalInformation()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodRemovePersonalInformationDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
// Add a comment with author information
int commentIndex = sheet.Comments.Add("A1");
sheet.Comments[commentIndex].Note = "Sample comment";
sheet.Comments[commentIndex].Author = "Test Author";
// Display original author information
Console.WriteLine("Before removal - Comment Author: " + sheet.Comments[commentIndex].Author);
// Remove personal information
wb.RemovePersonalInformation();
// Save the workbook
wb.Save("output.xlsx", SaveFormat.Xlsx);
// Reload to verify removal
Workbook wb2 = new Workbook("output.xlsx");
Console.WriteLine("After removal - Comment Author: " + wb2.Worksheets[0].Comments[commentIndex].Author);
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
