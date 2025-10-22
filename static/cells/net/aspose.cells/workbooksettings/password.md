##WorkbookSettings.Password
WorkbookSettings property. Represents Workbook file encryption password
## WorkbookSettings.Password property
Represents Workbook file encryption password.
```csharp
public string Password { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyPasswordDemo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
// Access the first worksheet and add some data
Worksheet sheet = wb.Worksheets[0];
sheet.Cells["C6"].PutValue("test encrypt.");
// Set password to protect the workbook
wb.Settings.Password = "xixi";
// Save the workbook
wb.Save("output_with_password.ods");
// Create load options with password to open the protected workbook
LoadOptions loadOptions = new LoadOptions();
loadOptions.Password = "xixi";
// Open the password-protected workbook
Workbook wbProtected = new Workbook("output_with_password.ods", loadOptions);
// Verify the data
Console.WriteLine("Cell value: " + wbProtected.Worksheets[0].Cells["C6"].Value);
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
