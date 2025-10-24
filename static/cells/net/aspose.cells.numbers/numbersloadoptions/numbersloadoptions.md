##NumbersLoadOptions.NumbersLoadOptions
NumbersLoadOptions constructor. Constructor
## NumbersLoadOptions constructor
Constructor.
```csharp
public NumbersLoadOptions()
```
### Examples
```csharp
using System;
using System.Globalization;
using Aspose.Cells;
using Aspose.Cells.Numbers;
namespace AsposeCellsExamples
{
public class NumbersLoadOptionsMethodCtorDemo
{
public static void Run()
{
// Create NumbersLoadOptions using constructor
NumbersLoadOptions loadOptions = new NumbersLoadOptions
{
// Set some common properties
Password = "secure123",
ParsingFormulaOnOpen = true,
CultureInfo = new CultureInfo("en-US"),
StandardFont = "Arial",
MemorySetting = MemorySetting.MemoryPreference
};
// Load workbook with the options
Workbook workbook = new Workbook("sample.numbers", loadOptions);
// Save as XLSX
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [NumbersLoadOptions](../)
* namespace [Aspose.Cells.Numbers](../../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../../)
