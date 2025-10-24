##LoadOptions.FontConfigs
LoadOptions property. Gets and sets individual font configs. Only works for the Workbook which uses this LoadOptions to load
## LoadOptions.FontConfigs property
Gets and sets individual font configs. Only works for the [`Workbook`](../../workbook/) which uses this [`LoadOptions`](../) to load.
```csharp
public IndividualFontConfigs FontConfigs { get; set; }
```
### Examples
```csharp
using System;
using System.Text;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class LoadOptionsPropertyFontConfigsDemo
{
public static void Run()
{
// Create load options with FontConfigs
TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
{
FontConfigs = new IndividualFontConfigs()
};
// Set some font substitution rules using the correct API
loadOptions.FontConfigs.SetFontSubstitutes("Arial", new string[] { "Times New Roman" });
loadOptions.FontConfigs.SetFontSubstitutes("Courier New", new string[] { "Consolas" });
// Load a CSV file with the specified options
Workbook workbook = new Workbook("sample.csv", loadOptions);
// Save the workbook to an Excel file
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [IndividualFontConfigs](../../individualfontconfigs/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
