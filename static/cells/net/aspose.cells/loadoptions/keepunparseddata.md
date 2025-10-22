##LoadOptions.KeepUnparsedData
LoadOptions property. Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true
## LoadOptions.KeepUnparsedData property
Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true.
```csharp
public bool KeepUnparsedData { get; set; }
```
### Remarks
For scenarios that user only needs to read some contents from template file and does not need to save the workbook back, set this property as false may improve performance, especially when using it together with some kind of LoadFilter,
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class LoadOptionsPropertyKeepUnparsedDataDemo
{
public static void Run()
{
// Create load options and set KeepUnparsedData to false
LoadOptions options = new LoadOptions();
options.KeepUnparsedData = false;
// Load workbook with options
Workbook workbook = new Workbook("example.xlsx", options);
// Access worksheet and demonstrate unparsed data is not kept
Worksheet worksheet = workbook.Worksheets[0];
Console.WriteLine("Cell A1 value: " + worksheet.Cells["A1"].Value);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
