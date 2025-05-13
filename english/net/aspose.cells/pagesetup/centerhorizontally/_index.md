---
title: PageSetup.CenterHorizontally
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represent if the sheet is printed centered horizontally
type: docs
url: /net/aspose.cells/pagesetup/centerhorizontally/
---
## PageSetup.CenterHorizontally property

Represent if the sheet is printed centered horizontally.

```csharp
public bool CenterHorizontally { get; set; }
```

### Examples

```csharp
// Called: pageSetup.CenterHorizontally = true;
public static void PageSetup_Property_CenterHorizontally()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Access the PageSetup object
            PageSetup pageSetup = worksheet.PageSetup;

            // Set the print order to DownThenOver
            pageSetup.Order = PrintOrderType.DownThenOver;

            // Set some other page setup properties for demonstration
            pageSetup.PrintArea = "A1:D10";
            pageSetup.PrintTitleRows = "$1:$1";
            pageSetup.PrintTitleColumns = "$A:$A";
            pageSetup.CenterHorizontally = true;
            pageSetup.CenterVertically = true;

            // Save the workbook
            workbook.Save("PrintOrderTypeExample.xlsx");

            return;
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


