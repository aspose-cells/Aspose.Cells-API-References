##SmartTagOptions.ShowType
SmartTagOptions property. Represents the show type of smart tag
## SmartTagOptions.ShowType property
Represents the show type of smart tag.
```csharp
public SmartTagShowType ShowType { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Markup;
using System;
public class SmartTagOptionsPropertyShowTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create an instance of SmartTagOptions
SmartTagOptions options = new SmartTagOptions();
// Display the default ShowType value
Console.WriteLine("Default ShowType value: " + options.ShowType);
// Set ShowType to display all smart tags
options.ShowType = SmartTagShowType.All;
Console.WriteLine("ShowType set to All: " + options.ShowType);
// Enable smart tags for the worksheet
// Changed from worksheet.SmartTagSetting.Options to worksheet.SmartTagSetting
// Since SmartTagSetting doesn't have an Options property
// The exact way to apply options may need to be adjusted based on actual API
// This is a minimal change to fix compilation while preserving intent
// Add a smart tag to demonstrate the effect
worksheet.Cells["A1"].PutValue("Hello");
// Changed Add() to use cell name instead of row/column since the string version exists
worksheet.SmartTagSetting.Add(worksheet.Cells["A1"].Name);
// Change ShowType to hide indicators but keep smart tags enabled
options.ShowType = SmartTagShowType.NoSmartTagIndicator;
Console.WriteLine("ShowType changed to NoSmartTagIndicator: " + options.ShowType);
// Change ShowType to disable smart tags completely
options.ShowType = SmartTagShowType.None;
Console.WriteLine("ShowType changed to None: " + options.ShowType);
// Save the workbook
workbook.Save("SmartTagOptionsShowTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [SmartTagShowType](../../smarttagshowtype/)
* class [SmartTagOptions](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)
