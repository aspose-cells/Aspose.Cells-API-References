##WorkbookSettings.WarningCallback
WorkbookSettings property. Gets or sets warning callback
## WorkbookSettings.WarningCallback property
Gets or sets warning callback.
```csharp
public IWarningCallback WarningCallback { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyWarningCallbackDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set the warning callback
workbook.Settings.WarningCallback = new WarningCallbackImplementation();
// Create a worksheet with a potential warning scenario (duplicate named range)
Worksheet sheet = workbook.Worksheets[0];
sheet.Cells["A1"].PutValue("Test");
// This will trigger a warning about duplicate name
int index1 = workbook.Worksheets.Names.Add("TestRange");
workbook.Worksheets.Names[index1].RefersTo = "=Sheet1!$A$1";
int index2 = workbook.Worksheets.Names.Add("TestRange");
workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$A$1";
// Save the workbook (will trigger warning callback)
workbook.Save("WarningCallbackExample.xlsx");
}
}
public class WarningCallbackImplementation : IWarningCallback
{
public void Warning(WarningInfo warningInfo)
{
Console.WriteLine($"Warning: {warningInfo.WarningType}, Description: {warningInfo.Description}");
}
}
}
```
### See Also
* interface [IWarningCallback](../../iwarningcallback/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
