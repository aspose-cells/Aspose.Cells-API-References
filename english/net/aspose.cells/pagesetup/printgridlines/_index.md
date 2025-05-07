---
title: PageSetup.PrintGridlines
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents if cell gridlines are printed on the page
type: docs
url: /net/aspose.cells/pagesetup/printgridlines/
---
## PageSetup.PrintGridlines property

Represents if cell gridlines are printed on the page.

```csharp
public bool PrintGridlines { get; set; }
```

### Examples

```csharp
// Called: wb.Worksheets[0].PageSetup.PrintGridlines = false;
[Test]
        public void Property_PrintGridlines()
        {
            Workbook wb = new Workbook();
            wb.Worksheets[0].Cells["C10"].PutValue("There should not exist gridlines in PrintView of this sheet");
            wb.Worksheets[0].PageSetup.PrintGridlines = false;
            wb.Save(Constants.checkPath + "N42595_GidLinesInPrintView.xlsb");
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


