##WorkbookSettings.BuildVersion
WorkbookSettings property. Specifies the incremental public release of the application
## WorkbookSettings.BuildVersion property
Specifies the incremental public release of the application.
```csharp
public string BuildVersion { get; set; }
```
### Examples
```csharp
using System;
using System.Globalization;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyBuildVersionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the WorkbookSettings
WorkbookSettings settings = workbook.Settings;
// Set basic settings
settings.Author = "Sample Author";
settings.CultureInfo = new CultureInfo("en-US");
// Demonstrate BuildVersion property
settings.BuildVersion = "2.5.0";
Console.WriteLine($"Build Version set to: {settings.BuildVersion}");
// Save the workbook
workbook.Save("BuildVersionDemo.xlsx");
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
