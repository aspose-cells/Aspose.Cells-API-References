##WorkbookSettings.RemovePersonalInformation
WorkbookSettings property. True if personal information can be removed from the specified workbook
## WorkbookSettings.RemovePersonalInformation property
True if personal information can be removed from the specified workbook.
```csharp
public bool RemovePersonalInformation { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyRemovePersonalInformationDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set RemovePersonalInformation to true
workbook.Settings.RemovePersonalInformation = true;
// Add some sample data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Email");
worksheet.Cells["A2"].PutValue("John Doe");
worksheet.Cells["B2"].PutValue("john@example.com");
// Save the workbook
string outputPath = "output_with_personal_info_removed.xlsx";
workbook.Save(outputPath);
// Load the saved workbook to verify the setting
Workbook loadedWorkbook = new Workbook(outputPath);
Console.WriteLine("RemovePersonalInformation setting: " +
loadedWorkbook.Settings.RemovePersonalInformation);
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
