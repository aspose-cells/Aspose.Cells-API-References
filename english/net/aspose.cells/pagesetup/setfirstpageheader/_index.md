---
title: PageSetup.SetFirstPageHeader
second_title: Aspose.Cells for .NET API Reference
description: PageSetup method. Sets a script formatting the first page header of an Excel file. Only effect in Excel 2007 when IsHFDiffFirst is true
type: docs
url: /net/aspose.cells/pagesetup/setfirstpageheader/
---
## PageSetup.SetFirstPageHeader method

Sets a script formatting the first page header of an Excel file. Only effect in Excel 2007 when IsHFDiffFirst is true.

```csharp
public void SetFirstPageHeader(int section, string headerScript)
```

| Parameter | Type | Description |
| --- | --- | --- |
| section | Int32 | 0: Left Section, 1: Center Section, 2: Right Section. |
| headerScript | String | Header format script. |

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetFirstPageHeaderWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Set first page header with section number and header text
            pageSetup.SetFirstPageHeader(2, "&CHeader Text");

            // Save the workbook
            workbook.Save("output.xlsx");
        }
    }
}
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


