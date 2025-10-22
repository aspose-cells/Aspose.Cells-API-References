##LoadOptions.Region
LoadOptions property. Gets or sets the regional settings used for the Workbook that will be loaded
## LoadOptions.Region property
Gets or sets the regional settings used for the Workbook that will be loaded.
```csharp
public CountryCode Region { get; set; }
```
### Remarks
The regional settings may be used for initializing some features for the workbook such as fonts, themes, and so on. For text based file formats, such as CSV, HTML, ..., the regional setting also will be used to detect number formats and parse text values to numeric or datetime values for cells. This setting will be kept for the instantiated workbook later, that is, [`Region`](../../workbooksettings/region/) of the workbook will use the same region with this property.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class LoadOptionsPropertyRegionDemo
{
public static void Run()
{
// Create load options for HTML file
LoadOptions loadOpts = new LoadOptions(LoadFormat.Html);
// Set the region to USA
loadOpts.Region = CountryCode.USA;
// Load the HTML file with the specified region settings
Workbook wb = new Workbook("example.html", loadOpts);
// Access the first worksheet
Worksheet ws = wb.Worksheets[0];
// Demonstrate region-specific formatting by checking a cell's style
Style style = ws.Cells["A1"].GetStyle();
Console.WriteLine("Font used in cell A1: " + style.Font.Name);
Console.WriteLine("Region used for loading: " + loadOpts.Region);
}
}
}
```
### See Also
* enum [CountryCode](../../countrycode/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
