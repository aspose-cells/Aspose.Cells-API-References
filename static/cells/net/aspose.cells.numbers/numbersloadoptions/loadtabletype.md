##NumbersLoadOptions.LoadTableType
NumbersLoadOptions property. Gets and sets the type of loading multiple tables in one worksheet
## NumbersLoadOptions.LoadTableType property
Gets and sets the type of loading multiple tables in one worksheet.
```csharp
public LoadNumbersTableType LoadTableType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Numbers;
namespace AsposeCellsExamples
{
public class NumbersLoadOptionsPropertyLoadTableTypeDemo
{
public static void Run()
{
// Create an instance of NumbersLoadOptions
NumbersLoadOptions loadOptions = new NumbersLoadOptions
{
// Demonstrate LoadTableType property usage
LoadTableType = LoadNumbersTableType.OneTablePerSheet,
// Other minimal required properties
Password = "password123",
ParsingFormulaOnOpen = true
};
// Load a Numbers file with the specified load options
Workbook workbook = new Workbook("sample.numbers", loadOptions);
// Save the workbook in XLSX format
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* enum [LoadNumbersTableType](../../loadnumberstabletype/)
* class [NumbersLoadOptions](../)
* namespace [Aspose.Cells.Numbers](../../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../../)
