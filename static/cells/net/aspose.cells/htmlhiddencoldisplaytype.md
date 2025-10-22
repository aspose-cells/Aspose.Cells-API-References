##Enum HtmlHiddenColDisplayType
Aspose.Cells.HtmlHiddenColDisplayType enum. Represents two types of showing the hidden columns in html
## HtmlHiddenColDisplayType enumeration
Represents two types of showing the hidden columns in html.
```csharp
public enum HtmlHiddenColDisplayType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Hidden | `0` | Hidden the hidden columns in html page. |
| Remove | `1` | Remove the hidden columns in html page. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class HtmlHiddenColDisplayTypeDemo
{
public static void HtmlHiddenColDisplayTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["A3"].PutValue("Jane");
worksheet.Cells["A4"].PutValue("Doe");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["B3"].PutValue(25);
worksheet.Cells["B4"].PutValue(35);
// Hide the second column
worksheet.Cells.HideColumn(1);
// Create HtmlSaveOptions and set the HiddenColDisplayType
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
saveOptions.HiddenColDisplayType = HtmlHiddenColDisplayType.Remove;
// Save the workbook to HTML format
workbook.Save("HtmlHiddenColDisplayTypeExample.html", saveOptions);
Console.WriteLine("Workbook saved as HTML with hidden columns removed.");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
