---
title: PageSetup.CenterVertically
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represent if the sheet is printed centered vertically
type: docs
url: /net/aspose.cells/pagesetup/centervertically/
---
## PageSetup.CenterVertically property

Represent if the sheet is printed centered vertically.

```csharp
public bool CenterVertically { get; set; }
```

### Examples

```csharp
// Called: pageSetup.CenterVertically = true;
public static void Property_CenterVertically()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Access the PageSetup object
            PageSetup pageSetup = worksheet.PageSetup;

            // Set the print order to DownThenOver
            pageSetup.Order = PrintOrderType.DownThenOver;

            // Set some other page setup properties for demonstration
            pageSetup.PrintArea = &quot;A1:D10&quot;;
            pageSetup.PrintTitleRows = &quot;$1:$1&quot;;
            pageSetup.PrintTitleColumns = &quot;$A:$A&quot;;
            pageSetup.CenterHorizontally = true;
            pageSetup.CenterVertically = true;

            // Save the workbook
            workbook.Save(&quot;PrintOrderTypeExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


