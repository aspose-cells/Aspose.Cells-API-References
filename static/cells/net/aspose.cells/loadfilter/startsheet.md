##LoadFilter.StartSheet
LoadFilter method. Prepares filter options before loading given worksheet. Users implementation of LoadFilter can change the LoadDataFilterOptions here to denote how to load data for this worksheet
## LoadFilter.StartSheet method
Prepares filter options before loading given worksheet. User's implementation of LoadFilter can change the LoadDataFilterOptions here to denote how to load data for this worksheet.
```csharp
public virtual void StartSheet(Worksheet sheet)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sheet | Worksheet | The worksheet to be loaded. There are only few properties can be used for the given worksheet object here because most data and properties have not been loaded. The available properties are: Name, Index, VisibilityType |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class LoadFilterMethodStartSheetWithWorksheetDemo
{
// Create a custom load filter class that extends LoadFilter
class CustomLoadFilter : LoadFilter
{
public override void StartSheet(Worksheet sheet)
{
Console.WriteLine($"Processing sheet: {sheet.Name}");
// You can add custom logic here to handle specific sheets
}
}
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Name = "TestSheet";
// Create an instance of our custom load filter
CustomLoadFilter loadFilter = new CustomLoadFilter();
try
{
// Call the StartSheet method with the worksheet parameter
loadFilter.StartSheet(worksheet);
Console.WriteLine("StartSheet method executed successfully");
// Add some data to demonstrate the sheet is accessible
worksheet.Cells["A1"].PutValue("StartSheet Demo");
worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());
}
catch (Exception ex)
{
Console.WriteLine($"Error executing StartSheet method: {ex.Message}");
}
// Save the result
workbook.Save("LoadFilterStartSheetDemo.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../../worksheet/)
* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
