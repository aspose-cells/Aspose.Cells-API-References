##AbstractTextLoadOptions.LoadStyleStrategy
AbstractTextLoadOptions property. Indicates the strategy to apply style for parsed values when converting string value to number or datetime
## AbstractTextLoadOptions.LoadStyleStrategy property
Indicates the strategy to apply style for parsed values when converting string value to number or datetime.
```csharp
public TxtLoadStyleStrategy LoadStyleStrategy { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class AbstractTextLoadOptionsPropertyLoadStyleStrategyDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set a custom style for demonstration
Style customStyle = workbook.CreateStyle();
customStyle.Font.Name = "Arial";
customStyle.Font.Size = 12;
customStyle.Font.Color = System.Drawing.Color.Blue;
customStyle.Pattern = BackgroundType.Solid;
customStyle.ForegroundColor = System.Drawing.Color.LightYellow;
// Apply the style to a cell
Cell cell = cells["A1"];
cell.PutValue("Sample Text");
cell.SetStyle(customStyle);
// Create CSV data
string csvData = "Data1,Data2\nValue1,Value2";
byte[] byteArray = Encoding.ASCII.GetBytes(csvData);
MemoryStream stream = new MemoryStream(byteArray);
// Create text load options with LoadStyleStrategy
TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
{
LoadStyleStrategy = TxtLoadStyleStrategy.BuiltIn
};
// Import the CSV data with the specified load options
cells.ImportCSV(stream, loadOptions, 0, 0);
// Save the workbook to demonstrate the result
workbook.Save("LoadStyleStrategyDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* enum [TxtLoadStyleStrategy](../../txtloadstylestrategy/)
* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
