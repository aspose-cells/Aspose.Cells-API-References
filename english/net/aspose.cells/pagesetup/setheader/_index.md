---
title: PageSetup.SetHeader
second_title: Aspose.Cells for .NET API Reference
description: PageSetup method. Sets a script formatting the header of an Excel file
type: docs
url: /net/aspose.cells/pagesetup/setheader/
---
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
// Called: pageSetup.SetHeader(1, "&P"); // Current page number
public static void Method_String_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Access the header/footer of the worksheet
            PageSetup pageSetup = worksheet.PageSetup;

            // Set the header with different HeaderFooterCommandType values
            pageSetup.SetHeader(0, "&T"); // Text
            pageSetup.SetHeader(1, "&P"); // Current page number
            pageSetup.SetHeader(2, "&N"); // Page count
            pageSetup.SetHeader(0, "&D"); // Current date
            pageSetup.SetHeader(1, "&T"); // Current time
            pageSetup.SetHeader(2, "&A"); // Sheet name
            pageSetup.SetHeader(0, "&F"); // File name without path
            pageSetup.SetHeader(1, "&Z"); // File path without file name
            pageSetup.SetHeader(2, "&G"); // Picture

            // Save the workbook
            workbook.Save("HeaderFooterCommandTypeExample.xlsx");
            workbook.Save("HeaderFooterCommandTypeExample.pdf");
            return;
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


