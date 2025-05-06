---
title: PageSetup.PrintErrors
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Specifies the type of print error displayed
type: docs
url: /net/aspose.cells/pagesetup/printerrors/
---
## PageSetup.PrintErrors property

Specifies the type of print error displayed.

```csharp
public PrintErrorsType PrintErrors { get; set; }
```

### Examples

```csharp
// Called: pageSetup.PrintErrors = PrintErrorsType.PrintErrorsDisplayed;
public static void Property_PrintErrors()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Access the PageSetup of the worksheet
            PageSetup pageSetup = worksheet.PageSetup;

            // Set different print error types
            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsBlank;
            workbook.Save(&quot;PrintErrorsBlank.xlsx&quot;);

            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsDash;
            workbook.Save(&quot;PrintErrorsDash.xlsx&quot;);

            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsDisplayed;
            workbook.Save(&quot;PrintErrorsDisplayed.xlsx&quot;);

            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsNA;
            workbook.Save(&quot;PrintErrorsNA.xlsx&quot;);

            return;
        }
```

### See Also

* enum [PrintErrorsType](../../printerrorstype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


