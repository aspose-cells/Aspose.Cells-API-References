##Enum LoadNumbersTableType
Aspose.Cells.Numbers.LoadNumbersTableType enum. Indicates type of loading tables when some tables are in a sheet
## LoadNumbersTableType enumeration
Indicates type of loading tables when some tables are in a sheet.
```csharp
public enum LoadNumbersTableType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| OneTablePerSheet | `1` |  |
| OverrideOtherTables | `2` |  |
| TileTables | `4` |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Numbers;
using System;
public class LoadNumbersTableTypeDemo
{
public static void LoadNumbersTableTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Create a new worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create an instance of NumbersLoadOptions
NumbersLoadOptions loadOptions = new NumbersLoadOptions();
// Set the LoadNumbersTableType property
loadOptions.LoadTableType = LoadNumbersTableType.OneTablePerSheet;
// Load a Numbers file with the specified load options
workbook = new Workbook("LoadNumbersTableTypeExample_original.numbers", loadOptions);
// Save the workbook to an Excel file
workbook.Save("LoadNumbersTableTypeExample.xlsx");
Console.WriteLine("Workbook loaded and saved successfully.");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Numbers](../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../)
