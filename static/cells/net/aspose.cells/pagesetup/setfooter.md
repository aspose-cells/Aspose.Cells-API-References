##PageSetup.SetFooter
PageSetup method. Sets a script formatting the footer of an Excel file
## PageSetup.SetFooter method
Sets a script formatting the footer of an Excel file.
```csharp
public void SetFooter(int section, string footerScript)
```
| Parameter | Type | Description |
| --- | --- | --- |
| section | Int32 | 0: Left Section, 1: Center Section, 2: Right Section. |
| footerScript | String | Footer format script. |
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
For example: "&amp;Arial,Bold&amp;8Footer Note"
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupMethodSetFooterWithInt32StringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.PageSetup.SetFooter(0, "Page &P");
worksheet.PageSetup.SetFooter(1, "&D");
worksheet.PageSetup.SetFooter(2, "&A");
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
