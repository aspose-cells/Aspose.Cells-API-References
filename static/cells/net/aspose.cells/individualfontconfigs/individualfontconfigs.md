##IndividualFontConfigs.IndividualFontConfigs
IndividualFontConfigs constructor. Ctor
## IndividualFontConfigs constructor
Ctor.
```csharp
public IndividualFontConfigs()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class IndividualFontConfigsMethodCtorDemo
{
public static void Run()
{
// Create load options with IndividualFontConfigs
var loadOptions = new OdsLoadOptions
{
FontConfigs = new IndividualFontConfigs(),
StandardFont = "Arial",
StandardFontSize = 12
};
// Create a new workbook with default worksheet
var workbook = new Workbook(FileFormatType.Xlsx);
// Access a worksheet and add some text
var worksheet = workbook.Worksheets[0];
var cell = worksheet.Cells["A1"];
cell.PutValue("Sample text with custom font configs");
// Save the workbook (load options aren't needed for saving)
workbook.Save("FontConfigsDemo.ods", SaveFormat.Ods);
}
}
}
```
### See Also
* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
