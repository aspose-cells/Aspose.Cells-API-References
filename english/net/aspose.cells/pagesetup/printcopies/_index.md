---
title: PageSetup.PrintCopies
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Get and sets number of copies to print
type: docs
url: /net/aspose.cells/pagesetup/printcopies/
---
## PageSetup.PrintCopies property

Get and sets number of copies to print.

```csharp
public int PrintCopies { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].PageSetup.PrintCopies, 1);
public void PageSetup_Property_PrintCopies()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Assert.AreEqual(workbook.Worksheets[0].PageSetup.PrintCopies, 1);
}
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


