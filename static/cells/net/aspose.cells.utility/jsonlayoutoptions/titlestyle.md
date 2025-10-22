##JsonLayoutOptions.TitleStyle
JsonLayoutOptions property. Gets and sets the style of the title
## JsonLayoutOptions.TitleStyle property
Gets and sets the style of the title.
```csharp
public Style TitleStyle { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;
namespace AsposeCellsExamples
{
public class JsonLayoutOptionsPropertyTitleStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Sample JSON data
string jsonInput = @"
{
""Name"": ""John"",
""Age"": 30,
""JoinDate"": ""2023-05-15""
}";
// Create custom style for titles
CellsFactory factory = new CellsFactory();
Style titleStyle = factory.CreateStyle();
titleStyle.HorizontalAlignment = TextAlignmentType.Center;
titleStyle.Font.Color = System.Drawing.Color.BlueViolet;
titleStyle.Font.IsBold = true;
// Configure JSON import options
JsonLayoutOptions options = new JsonLayoutOptions();
options.ArrayAsTable = true;
options.TitleStyle = titleStyle;
options.ConvertNumericOrDate = true;
options.DateFormat = "yyyy-MM-dd";
// Import JSON data with custom title style
JsonUtility.ImportData(jsonInput, worksheet.Cells, 0, 0, options);
// Auto-fit columns for better visibility
worksheet.AutoFitColumns();
// Save the workbook
workbook.Save("JsonWithStyledTitles.xlsx");
}
}
}
```
### See Also
* class [Style](../../../aspose.cells/style/)
* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)
