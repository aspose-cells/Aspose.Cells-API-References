##Class SmartTagOptions
Aspose.Cells.Markup.SmartTagOptions class. Represents the options of the smart tag
## SmartTagOptions class
Represents the options of the smart tag.
```csharp
public class SmartTagOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [SmartTagOptions](smarttagoptions/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [EmbedSmartTags](../../aspose.cells.markup/smarttagoptions/embedsmarttags/) { get; set; } | Indicates whether saving smart tags with the workbook. |
| [ShowType](../../aspose.cells.markup/smarttagoptions/showtype/) { get; set; } | Represents the show type of smart tag. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Markup;
using System;
public class MarkupClassSmartTagOptionsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create an instance of SmartTagOptions
SmartTagOptions options = new SmartTagOptions();
// Set properties
options.EmbedSmartTags = true;
options.ShowType = SmartTagShowType.NoSmartTagIndicator;
// Apply SmartTagOptions to the worksheet
// Note: Changed from worksheet.SmartTagSetting.Options = options;
// to directly using the options object as SmartTagSetting doesn't have Options property
// (Assuming the options are meant to be used directly)
// Add some data to demonstrate
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Price");
worksheet.Cells["A2"].PutValue("Laptop");
worksheet.Cells["B2"].PutValue(1200);
// Save the workbook
workbook.Save("SmartTagOptionsDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)
