##LoadOptions.Password
LoadOptions property. Gets and set the password of the workbook
## LoadOptions.Password property
Gets and set the password of the workbook.
```csharp
public string Password { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class LoadOptionsPropertyPasswordDemo
{
public static void Run()
{
// Create load options and set password
LoadOptions options = new LoadOptions();
options.Password = "test";
// Load password-protected workbook
Workbook workbook = new Workbook("protected.xlsx", options);
// Remove password protection after loading
workbook.Settings.Password = null;
// Save the unprotected workbook
workbook.Save("unprotected.xlsx");
}
}
}
```
### See Also
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
