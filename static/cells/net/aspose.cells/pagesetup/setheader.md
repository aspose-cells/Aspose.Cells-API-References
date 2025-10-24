##PageSetup.SetHeader
PageSetup method. Sets a script formatting the header of an Excel file
## PageSetup.SetHeader method
Sets a script formatting the header of an Excel file.
```csharp
public void SetHeader(int section, string headerScript)
```
| Parameter | Type | Description |
| --- | --- | --- |
| section | Int32 | 0: Left Section, 1: Center Section, 2: Right Section. |
| headerScript | String | Header format script. |
### Remarks
Script commands:
| **Command** | **Description** |
| --- | --- |
| &amp;P | Current page number |
| &amp;N | Page count |
| &amp;D | Current date |
| &amp;T | Current time |
| &amp;A | Sheet name |
| &amp;F | File name without path |
| &amp;"&lt;FontName&gt;" | Font name, for example: &amp;"Arial" |
| &amp;"&lt;FontName&gt;, &lt;FontStyle&gt;" | Font name and font style, for example: &amp;"Arial,Bold" |
| &amp;&lt;FontSize&gt; | Font size. If this command is followed by a plain number to be printed in the header, it will be separated from the font height with a space character. |
| &amp;K&lt;RRGGBB&gt; | Font color, for example(RED): &amp;KFF0000 |
| &amp;G | Image script |
For example: "&amp;Arial,Bold&amp;8Header Note"
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupMethodSetHeaderWithInt32StringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
PageSetup pageSetup = worksheet.PageSetup;
// Set different header sections with various commands
pageSetup.SetHeader(0, "&F"); // Left section - File name
pageSetup.SetHeader(1, "Page &P of &N"); // Center section - Page numbering
pageSetup.SetHeader(2, "&D"); // Right section - Date
workbook.Save("PageSetup_SetHeader_Example.xlsx");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
