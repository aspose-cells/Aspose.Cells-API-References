---
title: Enum HeaderFooterCommandType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.HeaderFooterCommandType enum. Represents the command type of header and footer
type: docs
url: /net/aspose.cells/headerfootercommandtype/
---
## HeaderFooterCommandType enumeration

Represents the command type of header and footer.

```csharp
public enum HeaderFooterCommandType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Text | `0` | The text. |
| CurrentPage | `1` | Current page number |
| Pagecount | `2` | Page count |
| CurrentDate | `3` | Current date |
| CurrentTime | `4` | Current time |
| SheetName | `5` | Sheet name |
| FileName | `6` | File name without path |
| FilePath | `7` | File path without file name |
| Picture | `8` | Picture |

### Examples

```csharp
[C#]

namespace Demos
{
    using Aspose.Cells;
    using System;

    public class HeaderFooterCommandTypeDemo
    {
        public static void HeaderFooterCommandTypeExample()
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
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


