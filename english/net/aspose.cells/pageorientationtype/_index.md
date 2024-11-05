---
title: Enum PageOrientationType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.PageOrientationType enum. Represents print orientation constants
type: docs
url: /net/aspose.cells/pageorientationtype/
---
## PageOrientationType enumeration

Represents print orientation constants.

```csharp
public enum PageOrientationType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Landscape | `0` | Landscape orientation |
| Portrait | `1` | Portrait orientation |

### Examples

```csharp
[C#]

namespace Demos
{
    using Aspose.Cells;
    using System;

    public class PageOrientationTypeDemo
    {
        public static void PageOrientationTypeExample()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the first worksheet in the workbook
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Access the PageSetup object of the worksheet
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Set the page orientation to Landscape
            pageSetup.Orientation = PageOrientationType.Landscape;
            
            // Save the workbook to a file
            workbook.Save("PageOrientationTypeExample_Landscape.xlsx");

            // Set the page orientation to Portrait
            pageSetup.Orientation = PageOrientationType.Portrait;
            
            // Save the workbook to a different file
            workbook.Save("PageOrientationTypeExample_Portrait.xlsx");

            return;
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


