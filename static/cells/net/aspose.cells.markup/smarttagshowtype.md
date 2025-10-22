##Enum SmartTagShowType
Aspose.Cells.Markup.SmartTagShowType enum. Represents the show type of the smart tag
## SmartTagShowType enumeration
Represents the show type of the smart tag.
```csharp
public enum SmartTagShowType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| All | `0` | Indicates that smart tags are enabled and shown |
| NoSmartTagIndicator | `1` | Indicates that the smart tags are enabled but the indicator not be shown. |
| None | `2` | Indicates that smart tags are disabled and not displayed. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Markup;
using System;
public class MarkupClassSmartTagShowTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Demonstrate all SmartTagShowType enum values
Console.WriteLine("SmartTagShowType values:");
Console.WriteLine($"All: {SmartTagShowType.All}");
Console.WriteLine($"NoSmartTagIndicator: {SmartTagShowType.NoSmartTagIndicator}");
Console.WriteLine($"None: {SmartTagShowType.None}");
// Create and configure a smart tag
var smartTagCollection = worksheet.SmartTagSetting.Add("urn:schemas-microsoft-com:office:smarttags#date");
// Set properties that would use SmartTagShowType (simulated since actual property isn't available)
Console.WriteLine("\nSmart tag created at A1 with current date");
// Save with different show type scenarios
workbook.Save("SmartTagShowTypeDemo_All.xlsx");
Console.WriteLine("Workbook saved with default show type (All)");
// Create another workbook with different show type behavior
Workbook workbook2 = new Workbook();
Worksheet worksheet2 = workbook2.Worksheets[0];
worksheet2.SmartTagSetting.Add("urn:schemas-microsoft-com:office:smarttags#date");
Console.WriteLine("\nSecond workbook created with smart tag at B2");
workbook2.Save("SmartTagShowTypeDemo_None.xlsx");
Console.WriteLine("Second workbook saved (simulating None behavior)");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)
