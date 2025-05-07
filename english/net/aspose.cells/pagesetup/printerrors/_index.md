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
// Called: AssertHelper.AreEqual(PrintErrorsType.PrintErrorsBlank, sheet.PageSetup.PrintErrors, "sheet.PageSetup.PrintErrors");
private void Property_PrintErrors(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[0];
            AssertHelper.AreEqual(PrintErrorsType.PrintErrorsBlank, sheet.PageSetup.PrintErrors, "sheet.PageSetup.PrintErrors");
        }
```

### See Also

* enum [PrintErrorsType](../../printerrorstype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


